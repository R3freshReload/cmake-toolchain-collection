# Windows Toolchains
## mingw-toolchain.cmake
This toolchain file will automatically download llvm-mingw-20241217 for the host platform and use it to build.
### Supported Target Architectures
To change the target arch you need to change the CMAKE_SYSTEM_PROCESSOR variable in the toolchain file to one of the following:
- aach64
- x86_64

### Supported Host Platforms
- Windows
  - x86_64
- Darwin
  - aarch64
  - x86_64
- Linux
  - x86_64
  - aarch64