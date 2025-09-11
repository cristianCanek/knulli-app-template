# Knulli app template

This repository is intended to be used as a template when creating applications targeted to run in [KNULLI](https://knulli.org/) using:

- [LVGL 9.3.0](https://lvgl.io/)
- [SDL 3](https://wiki.libsdl.org/SDL3)
- [OpenGL ES 2](https://www.khronos.org/opengles/)

## Prerequisites

Ensure you ahve installed the next packages before building the application:

    << TODO: List the dependencies here. >>

For convenience, use the next command(s):

```bash
sudo apt install ... -y

```

## Building the app

### Natively (in a Debian ARM64 setup)

    << TODO: Complete this section. >>

```bash
cmake -B build -S .
make -C build -j
```

### Cross-compiling (in a x32_64 Debian setup)

    << TODO: Complete this section. >>

## Runing the app

### Localy (for testing)

```bash
sudo build/bin/lvglsim -b sdl
```

### In a KNULLI device

    << TODO: Complete this section. >>
