Building Project Chrono:

1/4/17

Linux Build

**Note:** Built using CMake 3.6.3, Irrlicht 1.8.4, and GCC 6.2.1.

Dependencies:

1. Install CMake from: https://cmake.org/download/

2. GCC

3. Irrlicht (for compiling instructions see irrlicht.md)


Steps:

1. Make a directory for Chrono in your home directory such as /home/Chrono/

2. Clone Project Chrono from GitHub: https://github.com/projectchrono/chrono.git

	This should put the Chrono source code in the directory /home/Chrono/chrono/
	
3. It is suggested that you create a directory to build chrono in, such as /home/Chrono/build/

	You do not want to create the directory in /home/Chrono/chrono/ as it could be lost when pulling from GitHub.
	
4. Run CMake.

	Click "Browse Source..." and select the /home/Chrono/chrono/ directory.
	
	Click "Browse Build..." and select the /home/Chrono/build/ directory.
	
5. Click the "Configure" button.

	Options all highlighted in red should now appear.
	
	You will want to select "ENABLE_MODULE_FEA", "ENABLE_MODULE_IRRLICHT", "ENABLE_MODULE_POSTPROCESS", and "ENABLE_MODULE_VEHICLE" at the least.
	
	For instructions on how to compile the other modules, please refference the respective guide.
6. Click on the "Configure" button, again.

	If you compiled Irrlicht on your own, CMake should now through an error about not being able to find Irrlicht.
	
	In the CH_IRRLICHTDIR option, point to /home/irrlicht-x.x.x, or whatever path you installed it on.
	
	In the CH_IRRLICHTLIB option, point to /home/irrlicht-x.x.x/lib/Linux/libIrrlicht.so.1.8.4.
	
7. Hit "Configure" once again, then "Generate".

8. Finally, go to /home/Chrono/build/ and run a "make" to finish the build.
