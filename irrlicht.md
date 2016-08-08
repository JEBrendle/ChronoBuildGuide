Compiling Irrlicht 1.8.2:

1. To use GCC 4.9.4, add the line CXX = /”path to gcc”/ gcc-4.9.4-x86-64/bin/g++ above the compiler flags in the Makefile.
2. Add the flag “-fPIC” to the CXXFLAGS and CPPFLAGS in the Makefile.
3. Run a “make” in the directory /irrlicht-1.8.2/source/Irrlicht/.
4. Run a “make sharedlib” in the same directory. This creates libIrrlicht.so.1.8.2.
5. Since Chrono projects will look for libIrrlicht.so.1.8, we will create a symbolic link that will let Chrono find libIrrlicht.so.1.8 and use  libIrrlicht.so.1.8.2. To do this, use the command “ln -s ./libIrrlicht.so.1.8.2 ./libIrrlicht.so.1.8” in the directory “/irrlicht-1.8.2/lib/Linux/”
6. Irrlicht should now be good for use with Chrono.
 
