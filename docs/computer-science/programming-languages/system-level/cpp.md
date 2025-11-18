# C++

## CORE CONTENT

### Documentions

- [ISO C++](https://isocpp.org/)

### Compilers
|Compilers |Implementation Language|Runtime Enviromnet|
|:-----------:|:-----------------:|:----------------:|
|GCC          |C/C++                |Multiple OS|
|Clang        |C++                   |Multiple OS|
|MSVC          |C++                   |Windows, WSL|
|ICC/ICX       |C++                   |X86/ARM|
|PGI/NVIDIA HPC       |C++        |GPU/HPC|
|ARM Compiler       |C++        |ARM|
|TI C6000/CCS     |C++        |TI DSP|
|SDCC     |C        |8051/PIC|
|Emscripten     |C++       |WebAssembly|

### Compilers/Libc/STL Combination

|Platform|Compilers |STL|Libc|
|:----:|:----:|:----:|:----:|
|Linux|GCC |libstdc++|glibc|
|Linux Container|Clang |libc++ |musl|
|macOS/iOS|Clang |libc++|libkx|
|Windows|MSVC |MSVC STL|UCRT|
|Windows/GCC|MinGW |libstdc++|MSVCRT|
|Embedded|arm-none-eabi-gcc |libstdc++|Newlib|
|Android NDK|Clang |libc++|Bionic|
|Game Engine|Any |EASTL|Newlib/Custom|