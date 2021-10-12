# vscode-opengl-debug-setting
OpenGL C++ template for VS Code IDE.

This template is based on [https://github.com/vkphillia/opengl-cpp-template](https://github.com/vkphillia/opengl-cpp-template).

## Integrated OpenGL Libraries List

- GLFW
- GLAD
- GLM

## How to run this project

1.  Clone this repo
2.  Open this repo as a folder in Visual Studio Code
3.  In VSCode menu under `Run` option select `run without debugging` (or just `ctrl+alt+b`)

## Minimal setting

- set `c_cpp_properties.json`
  - change `"compilerPath": "C:\\msys64\\mingw64\\bin\\g++.exe"` into your own **g++** compiler
- set `launch.json`
  - change `"miDebuggerPath": "C:\\msys64\\mingw64\\bin\\gdb.exe"` into  your own **gdb** debugger

## Prerequisites

- VS Code
  - VS Code C/C++ extension
- MinGW
