Compiling Irrlicht 1.8.x:
1/4/17
Linux Build

Note: Compiled using GCC 6.2.1.

**NOTE** Irrlicht can also be built by installing through the root in some Linux distributions. This will work with Chrono and you will not have to take the following steps.
 
Building Irrlicht from source: 
1. Download the Irrlicht source code from: 
2. Go to the following directory: /home/irrlicht-1.8.x/source/Irrlicht/
	Add the flag “-fPIC” to the CXXFLAGS and CPPFLAGS in the Makefile.
3. Staying in that directory, run a "make" command.
	When the "make" has completed, run a "make sharedlib" to create libIrrlicht.so.1.8.2.
4. Irrlicht can now be used with Chrono.
 
