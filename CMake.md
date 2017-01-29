# CMake-NoteBook

## What is CMake

Cmake is a build system that uses a single script (defined in a CMakeLists.txt file) to generate appropriate platform-specific build scripts.

## Command Intro

* **cmake_minimum_required(VERSION x.x.x):** the specification of the minimum required CMake version.
* **project():** defines the name of the project. (this commands also accepts additional parameters and variables)
* **set():** create text variables. 
e.g.: 

        set (MY_VAR "hello"): create a variable MY_VAR with the value "hello"

        set (OTHER_VAR "${MY_VAR} world!"): to refer to the variable, simply enclose it in the round braces prepended by a dollar sign.
        
        set (SOURCE_FILES a.cpp b.cpp c.cpp): aggregate all project source files into a single variable.
        
        set (CMAKE_CXX_STANDARD 11): enable C++11 standard.
        
        set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++1y -Wall"): set up additional compiler-related settings in CMAKE_CXX_FLAGS:

* **include_directories()**: specify directories with header files. The compiler searches the headers in several predefined locations that are specific to the operating system.
* **add_executable (my_executable ${SOURCE_FILES})**: a build target defines an executable or a library that the CMake script helps you build.


        
[Reference](https://www.jetbrains.com/help/clion/2016.3/quick-cmake-tutorial.html)
 
