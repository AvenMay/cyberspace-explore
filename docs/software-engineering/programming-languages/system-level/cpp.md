# C++

## CORE CONTENT

### Documentions

- [ISO C++](https://isocpp.org/)

### Books

- [C++Primer 5th.pdf]({{ files_server }}/software-engineering/programming-languages/system-level/cpp/C++Primer%205th.pdf)
- [C++标准库 2nd.pdf]({{ files_server }}/software-engineering/programming-languages/system-level/cpp/C++%E6%A0%87%E5%87%86%E5%BA%93%202nd.pdf)
- [CMake Cookbook.pdf]({{ files_server }}/software-engineering/programming-languages/system-level/cpp/CMake%20Cookbook.pdf)
- [cpp-primer.7z]({{ files_server }}/software-engineering/programming-languages/system-level/cpp/cpp-primer.7z)
- [Effective C++ 3rd.epub]({{ files_server }}/software-engineering/programming-languages/system-level/cpp/Effective%20C++%203rd.epub)

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

## USE-CASES

### CLI/TUI Programming

### WebAssembly

### Network Programming

### Embedded
