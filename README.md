# Hydrogen

## Getting Dependencies

My GPU has OpenGL 4.6 (latest) support. 
That's what I will be using when I compile.
Other versions should work fine though.

Getting the dependencies downloaded so that the project can be
built should be as simple as:

```bash
mkdir build
cd build

conan install .. --build=missing
```

This will download dependencies and compile them.

## CLion Setup

Change your CMake build configuration folder to use `build/`. 
If you don't, you will get an error about not being able to find 
`conanbuildinfo.cmake` and it will create extraneous
build folders not in `.gitignore`. And that's no good.