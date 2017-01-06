Building the Chrono Python Module:
1/6/17
Linux Build

Note: CMake 3.6.3, GCC 6.2.1, Python 2.7.12, and Swig 3.0.10 are needed to compile this module.

Steps:
1. In CMake, make sure that the source code directory for Chrono and the build directory are still selected in their proper positions.
	Click on the "ENABLE_MODULE_PYTHON" check box.
	Click "Configure".
	
**NOTE**
For the following steps, you need to check the "Advanced" box directly below the build directory in order to see the options that are going to be changed.
	
2. CMake should automatically find your swig executable, but if it does not, you should now set the path to the executable in the "SWIG_EXECUTABLE" option and the path to the directory in the "SWIG_DIR" option.

3. If you also have Python3 on your machine, CMake will probably try to use that version. While Chrono is supposed to work with Python3 as well, it seems to work best with Python2.7, so that is what we will be using.

4. We will now set the proper paths to each directory/executable/library.
	Set the "PYTHON_EXECUTABLE" option to the executable. It should be similar to "/usr/bin/python2.7".
	Set the "PYTHON_INCLUDE_DIRECTORY" option to the proper directory. It should be similar to "/usr/include/python2.7".
	Set the "PYTHON_LIBRARY" option to the proper library. It should be similar to "/usr/lib64/libpython2.7.so".

5. Click on "Configure", then "Generate".

6. Go to the Chrono Build directory and run a "make".

7. In order to use the Python Module, you have to set PYTHONPATH. In CMake there is a log at the bottom of the window. Scroll up in that log until you see red text that begins with "To have access to the Chrono::Python wrapper modules..." Since we ran a make, we need to know the directory labeled "For modules in the BUILD tree:" It should be similar to "/home/Chrono/Chrono_Build/bin/".
	We will now set PYTHONPATH to that directory.
	In a terminal, run the command "export PYTHONPATH=/home/Chrono/Chrono_Build/bin/", substituting in the directory that you saw in CMake.
	
8. The Chrono Python Module is now ready to use.
