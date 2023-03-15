#cmake
CMake 是可以让软件跨平台编译的工具。它使用CMakelists.txt来定制C++程序整个编译流程。(可见C++程序编译流程)CMake的编译流程为

1. 写好[[CMakelists.txt]]
2. cmake path (path指向包含CMakelist.txt的目录)生成makefile
3. 使用make进行编译
