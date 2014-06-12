Experiments-In-Measuring-Classroom-Activity-Using-Image-Analysis
================================================================

This is the repository for ENGG4802 thesis project: Experiments in measuring classroom activity using image analysis

Programs/library needed
1) Visual Studio 2010/2012
2) OpenCV (any version will do)
You can download OpenCV at their website @ http://opencv.org/downloads.html

Installtion Steps

1. Click on the .exe and extract to the desired directory (Preferred directory in C:/)
2. This step is to set an environment variable. 
3. Start up a command window and enter (depending on your machine)
4. setx -m OPENCV_DIR C:\OpenCV\Build\x86\vc10     (suggested for Visual Studio 2010 - 32 bit Windows)
5. setx -m OPENCV_DIR C:\OpenCV\Build\x64\vc10     (suggested for Visual Studio 2010 - 64 bit Windows)
6. setx -m OPENCV_DIR C:\OpenCV\Build\x86\vc11     (suggested for Visual Studio 2012 - 32 bit Windows)
7. setx -m OPENCV_DIR C:\OpenCV\Build\x64\vc11     (suggested for Visual Studio 2012 - 64 bit Windows)
4. Next go to System Variables -> system PATH -> Path Editor and enter %OPENCV_DIR%\bin where OPENCV_DIR is your directory of your OpenCV
5. 
