Building The Chrono FSI Module:

1/4/17

Linux Build

**Note:** CMake 3.6.3 and GCC 6.2.1 were used to build Chrono.

Steps:

1. Check the box next to "ENABLE_MODULE_FSI".

2. Click on "Configure".

3. Click on "Generate".

4. Go to the directory that you decided to build Chrono in and run a “make” command.

5. The FSI module will be for use after this, but it should be noted that to run the full capability of the FSI module, it will be necessary to enable the Chrono Parallel module and download NVIDIA drivers.
