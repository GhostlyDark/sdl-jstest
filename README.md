sdl-jstest
==========

`sdl2-jstest` is a simple program that lets you find
out how many joysticks SDL2 detected on your system, how many
axes, buttons, hats and balls they have each. It also lets you test
the joysticks by displaying the events they send or by displaying
their current button, axis, hat or ball state.

EMG fork
========

This version of `sdl2-jstest` changed the following options:
```
--event
--list
```
The program now closes immediately after an event has been
detected and the information printed has been changed specifically
for use as part of the [Electron Mupen64Plus GUI](https://github.com/GhostlyDark/EMG).

Requirements
------------

sdl-jstest requires the following packages to build:

* cmake
* libsdl2-dev
* libncurses5-dev

Compilation
-----------

To compile type:
```
mkdir build
cd build
cmake ..
make
```

Options
-------
```
-h, --help                 Print this help
--version                  Print version number and exit
-l, --list                 Search for available joysticks and list their properties
-t, --test JOYNUM          Display a graphical representation of the current joystick state
-g, --gamecontroller IDX   Test GameController
-e, --event JOYNUM         Display the events that are received from the joystick
-r, --rumble JOYNUM        Test rumble effects on gamepad JOYNUM
```
