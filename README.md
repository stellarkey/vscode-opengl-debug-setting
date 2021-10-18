# vscode-opengl-debug-setting
OpenGL C++ template for VS Code IDE.

This template is based on [https://github.com/vkphillia/opengl-cpp-template](https://github.com/vkphillia/opengl-cpp-template).

## Prerequisites

- VS Code (with VS Code C/C++ extension)
- MinGW (32 bit, with **environment variables**)

## How to run this project

1.  Clone this repo
2.  Open this repo as a folder in Visual Studio Code
3.  In VSCode menu
    1.  under `Terminal` option select `run task`-`Build` (or just **`ctrl+shift+b`**)
    2.  under `Run` option select `run without debugging` (or just **`ctrl+alt+b`**)

## Integrated OpenGL Libraries List

- GLFW (32 bit)
- GLAD
- GLM

### Folder Structure


|                                           | `include/`                 | `lib/`                       | `lib-static/` | `src/` |
| ----------------------------------------- | -------------------------- | ---------------------------- | ------------- | ------ |
| [GLFW](http://www.glfw.org/download.html) | `GLFW/*`                   | `glfw3.dll`, `libglfw3dll.a` | `libglfw3.a`  |        |
| [GLAD](https://glad.dav1d.de/)            | `glad/*`,`KHR/*`, `glad.c` |                              |               |        |
| [GLM](https://github.com/g-truc/glm)      | `glm/*`                    |                              |               |        |

### How to add your own Libraries

- if you have any **header files**, add them to `include/`
- libraries
  - if you have any **dynamic libraries**, add them to `lib/`
  - if you have any **static libraries**, add them to `lib-static/`
  - add `-lyour_library`  into `args` list within `tasks.json`

