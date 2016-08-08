Chrono Parallel Module:
Note: CMake 3.5.2, Blaze 2.6, and GCC 4.9.4 were used to compile Chrono.
You will also need to have installed Cuda and Boost.

1. Check the box next to ENABLE_MODULE_PARALLEL.
2. Click on Configure.
3. Set the BLAZE_DIR to the upper level directory of Blaze.
4. Click on Configure, again.
5. Click on Generate.
6. Go to the directory that you decided to build Chrono in and run a “make” command.
7. Become a super user and run a “make install” command.
8. The Chrono Parallel module should now be ready to use.
