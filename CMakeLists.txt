cmake_minimum_required(VERSION 3.12)
project(cb_opencvtest)

set(CMAKE_CXX_STANDARD 11)

set(opencv_include_dir
        "D:\\OpenCV-3.0.0_Release_Codeblocks1710\\include"
        "D:\\OpenCV-3.0.0_Release_Codeblocks1710\\include\\opencv"
        "D:\\OpenCV-3.0.0_Release_Codeblocks1710\\include\\opencv2")

set(opencv_libs
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_calib3d300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_core300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_features2d300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_flann300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_hal300.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_highgui300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_imgcodecs300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_imgproc300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_ml300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_objdetect300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_photo300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_shape300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_stitching300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_superres300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_ts300.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_video300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_videoio300.dll.a"
        "D:/OpenCV-3.0.0_Release_Codeblocks1710/x86/mingw/lib/libopencv_videostab300.dll.a"
        )

add_executable(cb_opencvtest main.cpp)

include_directories(${PROJECT_NAME} ${opencv_include_dir})
target_link_libraries(${PROJECT_NAME} ${opencv_libs})
