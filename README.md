# The Maze

The Maze is a 3D Maze game that uses ray casting to render a 2D map into a 3D navigable world!

The Maze was written was written in C ussing SDL2 library. Deveploment was performed using Ubuntu 14.04 LTS - gcc (Ubuntu 4.8.4-2ubuntu1~14.04) 4.8.4

## About SDL2

Simple DirectMedia Layer is a cross-platform development library designed to provide low level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL and Direct3D. It is used by video playback software, emulators, and popular games including Valve's award winning catalog and many Humble Bundle games.

### Setup SDL2

To set up SDL2 development libraries on a Windows system using MinGW or a similar environment, follow these steps:

1. Download SDL2 Development Libraries

 Go to the SDL2 official website.
 Download the development libraries for Windows. Typically, you'll want the "SDL2-devel-2.x.x-mingw.tar.gz" package if you are using MinGW.

2. Extract the SDL2 Package

    Extract the downloaded SDL2-devel-2.x.x-mingw.tar.gz archive using a tool like 7-Zip or WinRAR.
    After extracting, you should see folders such as include, lib, and bin.

3. Set Up SDL2 for MinGW

    Copy Files:
        Include Files: Copy the contents of the include folder (which contains the SDL2 headers) to the MinGW include directory, typically located at C:\MinGW\include.
        Library Files: Copy the contents of the lib folder to the MinGW library directory, typically located at C:\MinGW\lib.
        DLL Files: Copy the SDL2.dll file from the bin folder to a location where your executable can access it (e.g., in the same directory as your compiled program or in the system path).

## Instalation

```sh
git clone https://github.com/Giddy-K/The-Maze.git
```

## Usage

* Execute ./maze or type make run
* Use up and down arrow keys to move forward and backward (keys w and s serve the same function)
* Use right and left arrow keys to turn the camera arround (keys d and a serve the same function)

## Compilation

```sh
gcc -Wall -Werror -Wextra -pedantic ./src/*.c -IC:\MinGW\include\SDL2 -LC:\MinGW\lib -lmingw32 -lSDL2main -lSDL2 -lm -o maze
```

After compiling, ensure that SDL2.dll is either in the same directory as your compiled executable or in a directory included in your system's PATH.
You can now run your program using ./maze (or maze.exe on Windows).

## Flowchart

![The Maze Flow Chart](https://i.imgur.com/t0MxNni.png)

## Demo

![The Maze Demo](./images/demo.gif)
