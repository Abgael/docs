# Sony PlayStation2 (PCSX2)

## Requirements

- CMake

## How to compile (for Windows x64 - Visual Studio 2017)

In addition to the requirement(s) listed above, you will also need Visual Studio 2017 installed in order for the following to work.

Enter the following commands (from the PCSX2 source directory):

    mkdir build
    cd build
    cmake .. -DLIBRETRO=ON -DCMAKE_BUILD_TYPE=Release -G"Visual Studio 15 2017 Win64"
    cmake --build . --target pcsx2_libretro --config Release
    
!!! Warning
    If it says 'Could not find named generator' or something to that effect, it means you might be using
    the wrong cmake version on Msys2/Mingw. Remove the regular 'cmake' package and try to install 'mingw-w64-x86_64-cmake' instead.

## How to compile (for Windows x64 - Visual Studio 2019)

In addition to the requirement(s) listed above, you will also need Visual Studio 2019 installed in order for the following to work.

Enter the following commands (from the Dolphin source directory):

    mkdir build
    cd build
    cmake .. -DLIBRETRO=ON -DCMAKE_BUILD_TYPE=Release -G"Visual Studio 17 2019 Win64"
    cmake --build . --target pcsx2_libretro --config Release

!!! Warning
    If it says 'Could not find named generator' or something to that effect, it means you might be using
    the wrong cmake version on Msys2/Mingw. Remove the regular 'cmake' package and try to install 'mingw-w64-x86_64-cmake' instead.
