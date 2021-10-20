# build.h - A C build system
The purpose of `build.h` is so that C developers do not have to struggle with learning Make, CMake, Meson, etc. and can just configure their build system in C.

## Usage
All you have to do is place the `build.h` file in your C project directory, and write a `build.c` file to configure it. To build the project, all you need to do is compile `build.c`, which can be done with:
```sh
gcc -o build build.c
```
or, if you have `make` installed, you can do:
```sh
make build
```
(The above command does not need a `Makefile`, it uses `make`'s implicit rules.)
Running `./build` will build the entire project.
