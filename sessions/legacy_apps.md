# How to deal with Legacy Apps & Android compatibility

Make former Windows CE apps run on 4.3 and 6.0.
I invite everyone that knows about compatibility issues or wants to share his problems and solutions
There will be an overview how we moved from javaME to android, discuss recent changes in power management of Android 6 and will talk about Alias Activities.
Everything should work without reflection.

# Discussion and possible solutions

* Use different flavors for different versions of your app, especially different java source files
* Using one abstract class or interface and concrete implementations based on the target platform
  * Compat class with target sdk annotations might help
* Create a library project, where common code is extracted
