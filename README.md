# vscode-opengl-debug-setting
OpenGL C++ template for VS Code IDE.

This template is based on [https://github.com/vkphillia/opengl-cpp-template](https://github.com/vkphillia/opengl-cpp-template).

## Integrated OpenGL Libraries List

- GLFW (32 bit)
- GLAD
- GLM

### Folder Structure


|                                           | `include/`       | `lib/`                       | `lib-static/` | `src/`   |
| ----------------------------------------- | ---------------- | ---------------------------- | ------------- | -------- |
| [GLFW](http://www.glfw.org/download.html) | `GLFW/*`         | `glfw3.dll`, `libglfw3dll.a` | `libglfw3.a`  |          |
| [GLAD](https://glad.dav1d.de/)            | `glad/*`,`KHR/*` |                              |               | `glad.c` |
| [GLM](https://github.com/g-truc/glm)      | `glm/*`          |                              |               |          |

## How to run this project

1.  Clone this repo
2.  Open this repo as a folder in Visual Studio Code
3.  In VSCode menu under `Run` option select `run without debugging` (or just `ctrl+alt+b`)

## Minimal setting

- set `launch.json`
  - change `"miDebuggerPath": "C:\\msys64\\mingw64\\bin\\gdb.exe"` into  your own **gdb** debugger
- (optional) set `c_cpp_properties.json`
  - change `"compilerPath": "C:\\msys64\\mingw64\\bin\\g++.exe"` into your own **g++** compiler

## Prerequisites

- VS Code (with VS Code C/C++ extension)
- MinGW (with environment variables)
