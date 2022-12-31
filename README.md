# CMake Tools

Quick test run of the CMake Tools VS Code extension.

## About CMake Tools

[CMake Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools) is a VS-Code Extension provided by Microsoft that provides a workflow for CMake-based projects.

CMake Tools do not provide support for CMake scripting hence I additionally have the extension[CMake twxs](https://marketplace.visualstudio.com/items?itemName=twxs.cmake) enabled, that provides CMake language support for VS-Code.

## About CMake

CMake is an open-source, cross-platform tool that uses compiler and platform independent configuration files to generate native build tool files specific to a certain compiler and platform.

In other words CMake can be used for cross-compiling, this means that the software is built on one system but intended to run on a different system. For example that the software is developed and built on a PC but in the end run in an embedded system such as a network switch or washing machine.

## Get Started with CMake Tools on Windows

These notes are based on the tutorial [Get started with CMake Tools on Linux](https://code.visualstudio.com/docs/cpp/CMake-linux)

Prerequisites:

- [Visual Studio Code](https://code.visualstudio.com/download) editor
- [C/C++ for Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cpptools) extension
- [CMake Tools](https://marketplace.visualstudio.com/items?itemName=ms-vscode.cmake-tools) extension
- [CMake](https://cmake.org/download/)
- A C++ compiler for example one of these
  - [Build Tools for Visual Studio](https://aka.ms/vs/17/release/vs_BuildTools.exe)
  - GCC from MniGW-w64 via [Chocolatey](https://community.chocolatey.org/packages/mingw)
- Knowledge on how to open a console (terminal) in Windows

It is not in the scope of this discussion on exact details to install the above. Google is your friend here if having trouble installing everything.

### Step 1 Check CMake Version

Check that there is a recent version of CMake available by typing the following in a console terminal (omit to type the $ it just place holder for the path shown in the console):

```txt
$ cmake --version
cmake version 3.25.1
```

Output should be a number like above or higher.

### Check Compiler

CMake will use an existing compiler so need to ensure that one is installed on the computer that runs CMake.

Check for Microsoft C++ compiler:

TBD

Check for GCC:

```txt
$ gcc --version
gcc.exe (x86_64-posix-seh-rev0, Built by MinGW-W64 project) 8.1.0
Copyright (C) 2018 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
```

### Run CMake Quick Start

Open Command Palette in Visual Studio Code `Ctrl + Shift + p` and run `CMake: Quick Start`.
