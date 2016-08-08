Chrono Python Module:
Note: CMake 3.5.2, GCC 4.9.4, Anaconda 3-4.1.11, and Python 3.5.2 were used to compile Chrono. Also, you will need to have installed swig.

1. Check the box next to ENABLE_MODULE_PYTHON.
2. Click on Configure.
3. Make sure that under SWIG_EXECUTABLE, CMake has found your swig. You may have to show it what directory to look in.
4. Click on Generate.
5. Go to the directory that you chose to build Chrono in and run a “make” command.
6. Become a super user and run a “make install” command.
7. It will be necessary to run an “export PYTHONPATH=/”directory of DLLs”/”, or if you are running anaconda, you can follow the next steps.
8. First, create an environment called something along the lines of “chronopython.” You can do this by using the command “conda create –name chronopython biopython.”
9. In the directory “/anaconda3/envs/chronopython/etc/conda/activate.d/” make a file called env_vars.sh.
10. Inside this file should be written:
“#!/bin/sh

export PYTHONPATH=/home/jbrendle/anaconda3/bin/DLLs/:/usr/local/lib/”
11. In the directory “/anaconda3/envs/chronopython/etc/conda/deactivate.d/” make a file called env_vars.sh.
12. Inside this file should be written:
“#!/bin/sh

export PYTHONPATH=/home/jbrendle/anaconda3/bin/DLLs/:/usr/local/lib/”
13. This allows for you to enter the environment chronopython and use the Chrono Python Module without having to establish PYTHONPATH frequently.
14. To activate chronopython enter the command “source activate chronopython.”
15. The Chrono Python Module should now be ready for use.
