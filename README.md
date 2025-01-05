# CMake Toolchains
This repository contains a collection of my CMake toolchain files. They are structured into folders that are named after the target platform that the toolchain files inside build. So all toolchain files in macos are used to build a macos binary.

## Design
The toolchain files are written in a way that they should fetch everything required to build on their own, except the README.md specifies some base requirements. e.g. the windows/mingw-toolchain.cmake automatically downloads mingw and uses it to compile. 

## Usage
To use a specific toolchain file you should consults the README.md inside the target folder as they should contain details, such as configurable variables, on the toolchain files in the same folder. But in general you can use them by running:
```bash
mkdir -p cmake-build
cd cmake-build
cmake -DCMAKE_TOOLCHAIN_FILE=path/to/toolchain-file.cmake ..
```
