# Android Studio productivity - lessons learned

Android Studio brings tons of keyboard shortcuts that helps developers to keep hands more on the keyboard rather than relying much on the mouse. The lesser you use the mouse, results in faster development.

Here are some general tips how to boost your productivity and get your development on a higher level.

![Android Studio](https://github.com/marsicdev/marsicdev.github.io/raw/master/images/as-logo.png "Android Studio logo")

Here are some general tips how to boost your productivity and get your development on a higher level.

### No more Tabs

There are many ways to navigate a project inside Android Studio that doesn’t necessarily include having to look through a list of tabs and figure out where you have to click next.

Switch tabs off. You don’t need tabs.

![No more Tabs](https://github.com/marsicdev/marsicdev.github.io/blob/master/images/as-setup-no-tabs.png)

### Distraction free mode

While you are coding you don't need in your sight all the small buttons and the line numbers that are around your editor. Actually, ask your self when was the last time that you looked at line number?

![Distraction free mode](https://github.com/marsicdev/marsicdev.github.io/raw/master/images/as-setup-destraction-free.png)

### Plugins

Plugins can help you to do some boring everyday things like implementing parcelable code or generating some other boilerplate code that you need to do often or even with navigation. So choose your plugins carefully as they are you weapon of choice. Here are some that I'm using:

- [ADB Idea](https://github.com/pbreault/adb-idea) - debug android app over Wi-Fi
- [Android WiFiADB](https://github.com/pedrovgs/AndroidWiFiADB) - debug android app over Wi-Fi
- [Inner Builder](https://github.com/analytically/innerbuilder) - adds a 'Builder' action to the Generate menu
- [CodeGlance](https://github.com/Vektah/CodeGlance) - displays a zoomed out overview or minimap
- [Android Parcelable](https://github.com/mcharmas/android-parcelable-intellij-plugin) - generates an Android Parcelable implementation based on fields in the class

### Shortcuts

Well, let us see some of the shortcuts for android studio for Mac user. If you get used to this shortcuts and remember them your coding and navigation will be peace of cake.

#### Default Android Studio Shortcuts

| Command Type     		                                                  | Shortcut                         |
|:------------------------------------------------------------------------|:--------------------------------:|
| Display list of available auto-fixes for code warning/error at cursor   | <kbd>Alt</kbd>+<kbd>Enter</kbd>  |
| Rename **all** copies of the variable/method/class at cursor            | <kbd>Shift</kbd>+<kbd>F6</kbd> |
| Generate code (incl. getters, setters, constructors, method overrides)  | <kbd>Cmd</kbd>+<kbd>N</kbd>  |
| Reformat code to conform to Android Studio's default style              | <kbd>Cmd</kbd>+<kbd>Alt</kbd>+<kbd>L</kbd>                |
| Comment/Uncomment all selected lines (also works in xml files)          | <kbd>Cmd</kbd>+<kbd>/</kbd>            |
| Find text in the current file                                           | <kbd>Cmd</kbd>+<kbd>F</kbd>           |
| Search for and open any file by name (filters as you type)              | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>O</kbd> |
| Search for and list **any** occurrences of text                         | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>F</kbd>      |
| Search for and go to any symbol (incl. variables and methods)           | <kbd>Alt</kbd>+<kbd>Cmd</kbd>+<kbd>O</kbd>                |
| Find and replace in current file                                        | <kbd>Cmd</kbd>+<kbd>R</kbd>            |
| Show available parameters for current method                            | <kbd>Cmd</kbd>+<kbd>P</kbd>            |
| Show class structure in pop-up                                          | <kbd>Cmd</kbd>+<kbd>F12</kbd>                     |
| List **all** usages of the variable/method/class at cursor              | <kbd>Cmd</kbd>+<kbd>Cmd</kbd>+<kbd>F7</kbd>  |
| List recently viewed files in pop-up                                    | <kbd>Cmd</kbd>+<kbd>E</kbd>                       |
| List recently edited files in pop-up                                    | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>E</kbd>                 |
| List implementations/overrides of class/interface/method at cursor      | <kbd>Cmd</kbd>+<kbd>Alt</kbd>+<kbd>B</kbd>                |
| View code hierarchy for symbol in pop-up                                | <kbd>Ctrl</kbd>+<kbd>Cmd</kbd>+<kbd>H</kbd>                |
| View full refactor menu                                                 | <kbd>Ctrl</kbd>+<kbd>T</kbd>                       |
| View javadoc of symbol at cursor in pop-up                              | <kbd>F1</kbd>                    |
| View definition of method at cursor in pop-up                           | <kbd>Cmd</kbd>+<kbd>Y</kbd>           |
| Skip back/forward through cursor position history                       | <kbd>Cmd</kbd>+<kbd>[</kbd>/<kbd>]</kbd> |
| Go to the declaration of the variable/method/class at cursor            | <kbd>Cmd</kbd>+<kbd>B</kbd>      |
| Go to given line number in current file                                 | <kbd>Cmd</kbd>+<kbd>L</kbd>                       |
| Go to next highlighted error in current file                            | <kbd>F2</kbd>                   |
| Move code line at cursor up/down                                        | <kbd>Alt</kbd>+<kbd>Shift</kbd>+<kbd>up</kbd>/<kbd>down</kbd>        |
| Move code block at cursor up/down                                       | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>up</kbd>/<kbd>down</kbd>        |
| Duplicate current line                                                  | <kbd>Cmd</kbd>+<kbd>D</kbd>                       |
| Complete statement (add braces, parentheses, semi-colon)                | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>Enter</kbd>             |
| Insert new line below current cursor position                           | <kbd>Shift</kbd>+<kbd>Enter</kbd>                     |
| Toggle **Project** sidebar Visibility                                   | <kbd>Cmd</kbd>+<kbd>1</kbd>                     |
| Toggle **Run** sidebar Visibility                                       | <kbd>Cmd</kbd>+<kbd>4</kbd>                     |
| Toggle **LogCat** sidebar Visibility                                    | <kbd>Cmd</kbd>+<kbd>6</kbd>                     |
| Build and Run                                                           | <kbd>Ctrl</kbd>+<kbd>R</kbd>            |
| Run                                                                     | <kbd>Cmd</kbd>+<kbd>F9</kbd>            |
| Debug                                                                   | <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>D</kbd>            |
| Clipboard history                                                       | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>V</kbd>            |
| Project settings                                                        | <kbd>Cmd</kbd>+<kbd>,</kbd>            |

#### Custom Android Studio Shortcuts

For some common repetitive everyday tasks I added some custom shortcuts

| Command Type                                                            | Shortcut                         |
|:------------------------------------------------------------------------|:--------------------------------:|
| Sync with Gradle                                                        | <kbd>Alt</kbd>+<kbd>Shift</kbd>+<kbd>S</kbd>            |
| Compare with same repository version                                    | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>D</kbd>            |
| Clean project                                                           | <kbd>Cmd</kbd>+<kbd>Shift</kbd>+<kbd>L</kbd>            |
| Duplicate line                                                          | <kbd>Ctrl</kbd>+<kbd>Cmd</kbd>+<kbd>down</kbd>            |
| Delete line                                                             | <kbd>Cmd</kbd>+<kbd>D</kbd>            |

### References

This leacture was all about lessons learned from different articles and talks from some really awesome Android developers.

#### Videos

* [Android Studio for Experts (Android Dev Summit 2015)](https://www.youtube.com/watch?v=Y2GC6P5hPeA)
* [Mouseless Driven Development by Hadi Hariri](https://vimeo.com/98922030)
* [The experts’ guide to Android development tools](https://www.youtube.com/watch?v=hHnTIMjd1Y8)

#### Articles

* [The powerful Android Studio](http://saulmm.github.io/the-powerful-android-studio) - Saúl Molinero
* [{dev} tips](https://medium.com/sebs-top-tips) - Sebastiano Poggi
* [No Tabs in IntelliJ IDEA](http://hadihariri.com/2014/06/24/no-tabs-in-intellij-idea/) - Hadi Hadiri
* [Android Studio tips of the day](http://www.developerphil.com/android-studio-tips-of-the-day-roundup-1/) - Developer Phil

#### Cheatsheet

* [IntelliJ IDEA Shortcuts Reference Card](https://resources.jetbrains.com/assets/products/intellij-idea/IntelliJIDEA_ReferenceCard_mac.pdf)
* [Presentations slides](http://marsic.info/files/AS_productivity-Marko_Arsic-DroidCon_Berlin_2016.pdf) containing all links already listed above

*Speaker:* [Marko Arsic](http://marsic.info/) ([@mArsic](https://twitter.com/marsic)) 
