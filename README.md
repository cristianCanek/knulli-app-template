# LVGL + SDL HelloWorld application

This repository is intended to be used as a hello world example when building applications in Linux (wether in a x32_64 or arm64 architecture) using [LVGL 9.3.0](https://lvgl.io/) + [SDL 2](https://wiki.libsdl.org/SDL2).


## Prerequisites

Ensure you have installed the next packages before building the application (for convenience, use the next command):

```bash
sudo apt install git cmake gcc g++ python3.13-venv pkg-config libsdl2-dev libsdl2-image-dev libglfw3-dev libglew-dev -y
```

Clone the repository with its submodules:

```bash
git clone --recursive https://github.com/cristianCanek/lvgl-sdl-helloworld.git
```


## Building the application

From the root path **within the lvgl-sdl-helloworld** repository, run these commands:

```bash
cmake -B build -S .
make -C build -j
```


## Running the application

```bash
# Running the application using the SDL backend (default size, 640x480)
sudo ./build/bin/lvglsim -b SDL
```

Also give it a try to the next commands:

```bash
# List supported backends (configured drivers)
sudo ./build/bin/lvglsim -B

# Print LVGL version
sudo ./build/bin/lvglsim -V

# Running the application with custom width and height
sudo ./build/bin/lvglsim -b SDL -W 300 -H 200
```
