In this post we are taking about common case that have very bad impact on android application memory. Knowing that leaking will definitely reduce average session time, as after using your app for a while it will crash very soon because of out of memory.
Let’s start by having a look to this code

public class ItemListFragment extends Fragment {
    private RecyclerView itemListRecyclerView;
    private ItemsAdapter itemsAdapter;
    @Override
    public void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        ...
        itemsAdapter = new ItemsAdapter(...);
    }
    @Override
    public void onViewCreated(View view, Bundle savedInstanceState) {
        super.onViewCreated(view, savedInstanceState);

        itemListRecyclerView = (RecyclerView) view.findViewById(...);
        itemListRecyclerView.setAdapter(itemsAdapter);
    }
    @Override
    public void onDestroyView() {
        super.onDestroyView();
        itemListRecyclerView = null;
    }
    @Override
    void onDestory(){
        super.onDestory();
        itemsAdapter = null;
    }
}
Do you notice anything wrong?! It's very simple fragment,  just keeping the adapter in memory as caching for loaded data.  This will be useful when this fragment is used in FragmentAdapter with ViewPager. But I am sorry to tell you that if user keep switching between pages, your app will crash after sometime because of OutOfMemory

Let have a deep look to this line itemListRecyclerView.setAdapter(itemsAdapter); 
The problem is that recycler view will register itself as observer for the Adapter. By checking the source code for recycler view root adapter, it has list of observers. So each time onViewCreated called the adapter will have reference of the newly created view (the whole hierarchy, as each view holds reference to its parent and so on).

Okay then what should be the solution, at the moment we can think of two ways

supper easy solution is to break the link between the adapter and the view by calling recyclerView.setAdapter(null) at onDestoryView. If you check android source code, this function checks for previous adapter and unregister itself from its observer list. which will solve the problem
second solution, is to move the caching role to the fragment (your controller or another appropriate class according to your caching mechanism), and reinitiate the adapter with each new view creation.  
Another two common cases for memory leaks are
ValueAnimator with repeatCount equals to INFINITE, in such case if you register any observer that holds reference to context (which is usually common). As Cheroographer object attached to current thread (UI thread) keeps reference to ValueAnimator.AnimationHandler which holds reference to object animator reference. As fix for this leak ValueAnimator end or cancel must be called. 
ViewTreeobserver observers 
Conclusion 

All mentioned cases are related to observer pattern implementation when dealing with android APIs. As a general advice when dealing with Android APIs when register any object as observer, make sure to unregister this object after completing your task. The common appropriate places to do this are 
Activity.onDestory
Fragment.onDestoryView or Fragment.onDestory
View.onDetachedFromView
RecyclerView.Adapter.onViewDetachedFromWindow
 


For better view and active links check http://hmware.blogspot.de/2015/10/android-and-memory-leaks.html