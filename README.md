# CMake Visual Studio 2017 Microsoft MPI Test
This is a minimal example of using CMake, C programming, MS MPI and Visual Studio that should
be able to be compiled on Windows, Mac and Linux with little or no modification.
##  Windows
#### Software required
- CMAKE-GUI (https://cmake.org/download/)
- Visual Studio 2017 (community version, free)

#### To compile
- download zip file of project and extract
- use cmake gui and
  - point cmake to source code and also specify the build to
    be in the same location as source but in build (i.e., source/build).
  - once configured, select generate, and then open project
  - once in Visual studio select helloworld as startup project 
  - then build 

## Linux
#### To compile
- open terminal (navigate to desired directory)
```
git clone https://github.com/PSUCompBio/cross-compiling-test
cd cross-compiling-test
mkdir build
cd bulid
ccmake ..
make -j8
```

## Mac OS
#### To compile
- open terminal (navigate to desired directory)
```
git clone https://github.com/PSUCompBio/cross-compiling-test
cd cross-compiling-test
mkdir build
cd bulid
ccmake ..
make -j8
```
