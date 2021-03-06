# OpenCV-MinGW-Build

MinGW 32bit and 64bit version of OpenCV compiled on Windows.

## MinGW32

### Compiling Environment

* MinGW-x32-5.3.0
* Windows-10-64bit
* CMake-3.9.2

### [OpenCV 3.4.1](https://github.com/huihut/OpenCV-MinGW-Build/tree/OpenCV-3.4.1)

```
git clone -b OpenCV-3.4.1 git@github.com:huihut/OpenCV-MinGW-Build.git
```

### [OpenCV 3.3.1](https://github.com/huihut/OpenCV-MinGW-Build/tree/OpenCV-3.3.1)

```
git clone -b OpenCV-3.3.1 git@github.com:huihut/OpenCV-MinGW-Build.git
```

## MinGW-w64

### Compiling Environment

* MinGW-x64-4.8.1-release-posix-seh-rev5
* Windows-10-64bit
* CMake-3.12.0

### [OpenCV 3.4.1-x64](https://github.com/huihut/OpenCV-MinGW-Build/tree/OpenCV-3.4.1-x64) 

```
git clone -b OpenCV-3.4.1-x64 git@github.com:huihut/OpenCV-MinGW-Build.git
```

<details><summary>Configuration</summary> 

```
General configuration for OpenCV 3.4.1 =====================================
  Version control:               unknown

  Platform:
    Timestamp:                   2018-07-31T02:14:11Z
    Host:                        Windows 10.0.17134 AMD64
    CMake:                       3.12.0
    CMake generator:             MinGW Makefiles
    CMake build tool:            E:/MinGW-w64/x64-4.8.1-release-posix-seh-rev5/mingw64/bin/mingw32-make.exe
    Configuration:               Release

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3
      requested:                 SSE3
    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2
      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      SSE4_1 (3 files):          + SSSE3 SSE4_1
      SSE4_2 (1 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
      FP16 (2 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
      AVX (5 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
      AVX2 (9 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2

  C/C++:
    Built as dynamic libs?:      YES
    C++11:                       YES
    C++ Compiler:                E:/MinGW-w64/x64-4.8.1-release-posix-seh-rev5/mingw64/bin/g++.exe  (ver 4.8.1)
    C++ flags (Release):         -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
    C++ flags (Debug):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  E:/MinGW-w64/x64-4.8.1-release-posix-seh-rev5/mingw64/bin/gcc.exe
    C flags (Release):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-narrowing -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
    C flags (Debug):             -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-narrowing -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      -Wl,--gc-sections  
    Linker flags (Debug):        -Wl,--gc-sections  
    ccache:                      NO
    Precompiled headers:         NO
    Extra dependencies:          opengl32 glu32
    3rdparty dependencies:

  OpenCV modules:
    To be built:                 calib3d core dnn features2d flann highgui imgcodecs imgproc java_bindings_generator ml objdetect photo python_bindings_generator shape stitching superres ts video videoio videostab
    Disabled:                    js world
    Disabled by dependency:      -
    Unavailable:                 cudaarithm cudabgsegm cudacodec cudafeatures2d cudafilters cudaimgproc cudalegacy cudaobjdetect cudaoptflow cudastereo cudawarping cudev java python2 python3 viz
    Applications:                tests perf_tests apps
    Documentation:               NO
    Non-free algorithms:         NO

  Windows RT support:            NO

  GUI: 
    Win32 UI:                    YES
    OpenGL support:              YES (opengl32 glu32)
    VTK support:                 NO

  Media I/O: 
    ZLib:                        build (ver 1.2.11)
    JPEG:                        build (ver 90)
    WEBP:                        build (ver encoder: 0x020e)
    PNG:                         build (ver 1.6.34)
    TIFF:                        build (ver 42 - 4.0.9)
    JPEG 2000:                   build (ver 1.900.1)
    OpenEXR:                     build (ver 1.7.1)

  Video I/O:
    Video for Windows:           YES
    DC1394:                      NO
    FFMPEG:                      YES (prebuilt binaries)
      avcodec:                   YES (ver 57.107.100)
      avformat:                  YES (ver 57.83.100)
      avutil:                    YES (ver 55.78.100)
      swscale:                   YES (ver 4.8.100)
      avresample:                YES (ver 3.7.0)
    GStreamer:                   NO
    DirectShow:                  YES

  Parallel framework:            none

  Trace:                         YES (built-in)

  Other third-party libraries:
    Lapack:                      NO
    Eigen:                       NO
    Custom HAL:                  NO
    Protobuf:                    build (3.5.1)

  NVIDIA CUDA:                   NO

  OpenCL:                        YES (no extra features)
    Include path:                E:/opencv_341/opencv/sources/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  Python (for build):            E:/Python37-32/python.exe

  Java:                          
    ant:                         NO
    JNI:                         C:/Program Files (x86)/Java/jdk1.8.0_181/include C:/Program Files (x86)/Java/jdk1.8.0_181/include/win32 C:/Program Files (x86)/Java/jdk1.8.0_181/include
    Java wrappers:               NO
    Java tests:                  NO

  Matlab:                        NO

  Install to:                    E:/opencv_341/opencv_mingw64_build/install
-----------------------------------------------------------------
```

</details>

### [OpenCV 4.0.0-alpha-x64](https://github.com/huihut/OpenCV-MinGW-Build/tree/OpenCV-4.0.0-alpha-x64)

```
git clone -b OpenCV-4.0.0-alpha-x64 git@github.com:huihut/OpenCV-MinGW-Build.git
```

<details><summary>Configuration</summary> 

```
General configuration for OpenCV 4.0.0-alpha =====================================
  Version control:               unknown

  Platform:
    Timestamp:                   2018-09-25T08:37:52Z
    Host:                        Windows 10.0.17134 AMD64
    CMake:                       3.12.0
    CMake generator:             MinGW Makefiles
    CMake build tool:            E:/MinGW-w64/x64-4.8.1-release-posix-seh-rev5/mingw64/bin/mingw32-make.exe
    Configuration:               Release

  CPU/HW features:
    Baseline:                    SSE SSE2 SSE3
      requested:                 SSE3
    Dispatched code generation:  SSE4_1 SSE4_2 FP16 AVX AVX2
      requested:                 SSE4_1 SSE4_2 AVX FP16 AVX2 AVX512_SKX
      SSE4_1 (4 files):          + SSSE3 SSE4_1
      SSE4_2 (2 files):          + SSSE3 SSE4_1 POPCNT SSE4_2
      FP16 (1 files):            + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 AVX
      AVX (6 files):             + SSSE3 SSE4_1 POPCNT SSE4_2 AVX
      AVX2 (10 files):           + SSSE3 SSE4_1 POPCNT SSE4_2 FP16 FMA3 AVX AVX2

  C/C++:
    Built as dynamic libs?:      YES
    C++ Compiler:                E:/MinGW-w64/x64-4.8.1-release-posix-seh-rev5/mingw64/bin/g++.exe  (ver 4.8.1)
    C++ flags (Release):         -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -O3 -DNDEBUG  -DNDEBUG
    C++ flags (Debug):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wundef -Winit-self -Wpointer-arith -Wshadow -Wsign-promo -Wuninitialized -Winit-self -Wno-narrowing -Wno-delete-non-virtual-dtor -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -fvisibility-inlines-hidden -g  -O0 -DDEBUG -D_DEBUG
    C Compiler:                  E:/MinGW-w64/x64-4.8.1-release-posix-seh-rev5/mingw64/bin/gcc.exe
    C flags (Release):           -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-narrowing -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -O3 -DNDEBUG  -DNDEBUG
    C flags (Debug):             -fsigned-char -W -Wall -Werror=return-type -Werror=non-virtual-dtor -Werror=address -Werror=sequence-point -Wformat -Werror=format-security -Wmissing-declarations -Wmissing-prototypes -Wstrict-prototypes -Wundef -Winit-self -Wpointer-arith -Wshadow -Wuninitialized -Winit-self -Wno-narrowing -Wno-comment -fdiagnostics-show-option -Wno-long-long -fomit-frame-pointer -ffunction-sections -fdata-sections  -msse -msse2 -msse3 -fvisibility=hidden -g  -O0 -DDEBUG -D_DEBUG
    Linker flags (Release):      -Wl,--gc-sections  
    Linker flags (Debug):        -Wl,--gc-sections  
    ccache:                      NO
    Precompiled headers:         NO
    Extra dependencies:
    3rdparty dependencies:

  OpenCV modules:
    To be built:                 calib3d core dnn features2d flann highgui imgcodecs imgproc java_bindings_generator ml objdetect photo python_bindings_generator shape stitching superres ts video videoio videostab
    Disabled:                    js world
    Disabled by dependency:      -
    Unavailable:                 java python2 python3 viz
    Applications:                tests perf_tests apps
    Documentation:               NO
    Non-free algorithms:         NO

  Windows RT support:            NO

  GUI: 
    Win32 UI:                    YES
    VTK support:                 NO

  Media I/O: 
    ZLib:                        build (ver 1.2.11)
    JPEG:                        build-libjpeg-turbo (ver 1.5.3-62)
    WEBP:                        build (ver encoder: 0x020e)
    PNG:                         build (ver 1.6.34)
    TIFF:                        build (ver 42 - 4.0.9)
    JPEG 2000:                   build (ver 1.900.1)
    OpenEXR:                     build (ver 1.7.1)
    HDR:                         YES
    SUNRASTER:                   YES
    PXM:                         YES
    PFM:                         YES

  Video I/O:
    Video for Windows:           YES
    DC1394:                      NO
    FFMPEG:                      YES (prebuilt binaries)
      avcodec:                   YES (ver 58.18.100)
      avformat:                  YES (ver 58.12.100)
      avutil:                    YES (ver 56.14.100)
      swscale:                   YES (ver 5.1.100)
      avresample:                YES (ver 4.0.0)
    GStreamer:                   NO
    DirectShow:                  YES

  Parallel framework:            none

  Trace:                         YES (built-in)

  Other third-party libraries:
    Lapack:                      NO
    Eigen:                       NO
    Custom HAL:                  NO
    Protobuf:                    build (3.5.1)

  OpenCL:                        YES (no extra features)
    Include path:                E:/opencv-4.0.0-alpha/opencv-4.0.0-alpha/3rdparty/include/opencl/1.2
    Link libraries:              Dynamic load

  Python (for build):            E:/Python37-32/python.exe

  Java:                          
    ant:                         NO
    JNI:                         C:/Program Files (x86)/Java/jdk1.8.0_181/include C:/Program Files (x86)/Java/jdk1.8.0_181/include/win32 C:/Program Files (x86)/Java/jdk1.8.0_181/include
    Java wrappers:               NO
    Java tests:                  NO

  Install to:                    E:/opencv-4.0.0-alpha/opencv-4.0.0-mingw64-build/install
-----------------------------------------------------------------
```

</details>

## How to compile OpenCV

* [blog.huihut . OpenCV使用CMake和MinGW的编译安装及其在Qt配置运行](https://blog.huihut.com/2017/12/03/CompiledOpenCVRunInQt/)
* [wiki.qt . How to setup Qt and openCV on Windows](https://wiki.qt.io/How_to_setup_Qt_and_openCV_on_Windows)
* [Tutorial: Installation from source for Windows with Mingw-w64](http://visp-doc.inria.fr/doxygen/visp-daily/tutorial-install-win10-mingw64.html)

## Using OpenCV in Visual Studio Code

[Running a C++ program with OpenCV 3.4.1 using MinGW-w64 g++ in Visual Studio Code on Windows 10 x64](https://stackoverflow.com/questions/51622111/opencv-c-mingw-vscode-fatal-error-to-compile/51801863#51801863)

## Using OpenCV in Qt

Add OpenCV library file and include path to Qt `.pro` file.

* My version of OpenCV : `OpenCV 3.3.1`
* My OpenCV path : `E:\OpenCV_3.3.1\OpenCV-MinGW-Build`

So the configuration is as follows (**You need to modify it according to your OpenCV.**) :

```
win32 {
INCLUDEPATH += E:\OpenCV_3.3.1\OpenCV-MinGW-Build\include
LIBS += E:\OpenCV_3.3.1\OpenCV-MinGW-Build\bin\libopencv_*.dll
}
```

or

```
win32 {
INCLUDEPATH += E:\OpenCV_3.3.1\OpenCV-MinGW-Build\include
LIBS += -LE:\OpenCV_3.3.1\OpenCV-MinGW-Build\bin \
    -llibopencv_calib3d331 \
    -llibopencv_core331 \
    -llibopencv_dnn331 \
    -llibopencv_features2d331 \
    -llibopencv_flann331 \
    -llibopencv_highgui331 \
    -llibopencv_imgcodecs331 \
    -llibopencv_imgproc331 \
    -llibopencv_ml331 \
    -llibopencv_objdetect331 \
    -llibopencv_photo331 \
    -llibopencv_shape331 \
    -llibopencv_stitching331 \
    -llibopencv_superres331 \
    -llibopencv_video331 \
    -llibopencv_videoio331 \
    -llibopencv_videostab331
}
```