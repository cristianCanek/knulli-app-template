# LVGL + SDL HelloWorld application

This repository is intended to be used as a hello world example when building applications in Linux (wether in a x32_64 or arm64 architecture) using [LVGL 9.3.0](https://lvgl.io/) + [SDL 2](https://wiki.libsdl.org/SDL2).


## Prerequisites

Ensure you have installed the next packages before building the application:

    << TODO: List the dependencies here. >>

For convenience, use the next command(s):

```bash
sudo apt install ... -y
```


## Building the app

```bash
cmake -B build -S .
make -C build -j
```


## Runing the app

```bash
# Running the app using the SDL backend (default size, 640x480)
sudo ./build/bin/lvglsim -b SDL
```

Also give it a try to the next commands:

```bash
# List supported backends (configured drivers)
sudo ./build/bin/lvglsim -B

# Print LVGL version
sudo ./build/bin/lvglsim -V

# Running the app with custom width and height
sudo ./build/bin/lvglsim -b SDL -W 300 -H 200
```