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
9. Next is to install Visual Studio.
10. Launch Visual Studio -> Win32 Console Application
11. They can be found in the Property Manager (View -> Property Pages)
12. Right click on Debug and add new project property sheet (this can be reuse for future OpenCV projects)
13. Select the sheet. Right Click -> Properties.
14. Go under C++ groups General entry and under "Additional Include Directories" add the path to your OpenCV include
15. $(OPENCV_DIR)\..\..\include
16. Next go to Linker -> General and under "Additional Library Directories" and add the libs directory
17. $(OPENCV_DIR)\lib
18. Then go to Linker -> Input and under "Additional Library Directories" entry and add the name of all modules which you want to use
19. The names of libraries are as follows: opencv_(The Name of the modules)(The version Number of the library you use)d.lib
20. A full list would look like this
21. opencv_core231d.lib
22. opencv_imgproc231d.lib
23. opencv_highgui231d.lib
24. opencv_ml231d.lib
25. opencv_video231d.lib
26. opencv_features2d231d.lib
27. opencv_calib3d231d.lib
28. opencv_objdetect231d.lib
29. opencv_contrib231d.lib
30.opencv_legacy231d.lib
32. opencv_flann231d.lib
33. The d at the end means these libraries required for the debug mode.
34. After that paste the Thesis source code and it will work



