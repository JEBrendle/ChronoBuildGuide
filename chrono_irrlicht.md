Chrono Irrlicht Module
Note: This was done using CMake 3.5.2 and Irrlicht 1.8.2.

1. In CMake, make sure that the check box for ENABLE_MODULE_IRRLICHT is checked.
2. Click on Configure.
3. Set CH_IRRLICHTDIR to the Irrlicht. Ex: /home/irrlicht-1.8.2.
4. Set CH_IRRLICHTLIB to the shared object that was created in the Irrlicht configuration. Ex: /irrlicht-1.8.2/lib/Linux/libirrlicht.so.1.8.2.
5. Click on advanced, and then add “-fPIC” to CMAKE_CXX_FLAGS.
6. Click on Configure, again.
7. Click on Generate.
8. Go to the directory in which you chose to build Chrono and run a “make” command.
9. When the make has completed, become a super user and run a “make install” command.
10. Exit the super user, and the Chrono Irrlicht Module should be ready for use.
11. Note: When running Chrono for the first time from a terminal, it may be necessary to set run the command “export LD_LIBRARY_PATH=/”path to Irrlicht shared object file”./

