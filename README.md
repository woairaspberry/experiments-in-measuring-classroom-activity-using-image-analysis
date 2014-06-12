Experiments-In-Measuring-Classroom-Activity-Using-Image-Analysis
================================================================

This is the repository for ENGG4802 thesis project: Experiments in measuring classroom activity using image analysis

Programs/library needed
1) Visual Studio 2010/2012
2) OpenCV (any version will do)
You can download OpenCV at their website @ http://opencv.org/downloads.html

Installtion Steps

1. Click on the OpenCV .exe and extract to the desired directory (Preferred directory in C:/)
2. This step is to set an environment variable. 
3. Start up a command window and enter (depending on your machine)
4. setx -m OPENCV_DIR C:\OpenCV\Build\x86\vc10     (suggested for Visual Studio 2010 - 32 bit Windows)
5. setx -m OPENCV_DIR C:\OpenCV\Build\x64\vc10     (suggested for Visual Studio 2010 - 64 bit Windows)
6. setx -m OPENCV_DIR C:\OpenCV\Build\x86\vc11     (suggested for Visual Studio 2012 - 32 bit Windows)
7. setx -m OPENCV_DIR C:\OpenCV\Build\x64\vc11     (suggested for Visual Studio 2012 - 64 bit Windows)
8. Next go to System Variables -> system PATH -> Path Editor and enter %OPENCV_DIR%\bin


How to build applications with OpenCV inside Visual Studio (VS)
1. VS has two build modes, Release and a Debig mode (choose one of them)
2. They can be found in the Property Manager (View -> Property Pages)
3. Right click on Debug and add new project property sheet (this can be reuse for future OpenCV projects)
4. Select the sheet. Right Click -> Properties.
5. Go under C++ groups General entry and under "Additional Include Directories" add the path to your OpenCV include
6. $(OPENCV_DIR)\..\..\include
6. Next go to Linker -> General and under "Additional Library Directories" and add the libs directory
7. $(OPENCV_DIR)\lib
8. Then go to Linker -> Input and under "Additional Library Directories" entry and add the name of all modules which you want to use
9. The names of libraries are as follows: opencv_(The Name of the modules)(The version Number of the library you use)d.lib
10. A full list would look like this
11. opencv_core231d.lib
opencv_imgproc231d.lib
opencv_highgui231d.lib
opencv_ml231d.lib
opencv_video231d.lib
opencv_features2d231d.lib
opencv_calib3d231d.lib
opencv_objdetect231d.lib
opencv_contrib231d.lib
opencv_legacy231d.lib
opencv_flann231d.lib
12. The d at the nd means these libraries required for the debug mode.
