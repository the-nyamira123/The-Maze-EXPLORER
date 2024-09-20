
The-Maze-EXPLORER
The Maze Explorer is a 3D maze game that uses raycasting to transform a 2D map into a fully navigable 3D world.

The game is built in C using the SDL2 library. Development was primarily done on Ubuntu 14.04 LTS using GCC (version 4.8.4-2ubuntu1~14.04).

About SDL2
SDL2 (Simple DirectMedia Layer) is a cross-platform development library that provides low-level access to audio, keyboard, mouse, joystick, and graphics hardware via OpenGL and Direct3D. It is widely used in video playback software, emulators, and several popular games, including Valve's award-winning catalog and many Humble Bundle games.

Setting Up SDL2 on Windows
To configure SDL2 development libraries on a Windows machine (using MinGW or a similar environment), follow these steps:

Download SDL2 Development Libraries
Head over to the official SDL2 website and download the SDL2 development libraries for Windows. If using MinGW, you'll likely need the SDL2-devel-2.x.x-mingw.tar.gz package.

Extract the SDL2 Package
Use tools like 7-Zip or WinRAR to extract the SDL2-devel-2.x.x-mingw.tar.gz archive. Once extracted, you'll have folders like include, lib, and bin.

Configure SDL2 for MinGW

Header Files: Copy the contents of the include folder (SDL2 headers) into the MinGW include directory, usually located at C:\MinGW\include.
Library Files: Copy the files from the lib folder to MinGW’s lib directory, usually at C:\MinGW\lib.
DLL Files: Place the SDL2.dll from the bin folder either in the same directory as your executable or in a system path location accessible by the program.
Installation
Clone the repository:

bash
Copy code
git clone https://github.com/the-nyamira123/The-Maze-EXPLORER.git
Usage
To run the game:

Execute the binary with ./maze or type make run.
Controls:

Move: Use the up/down arrow keys or W/S keys.
Rotate Camera: Use the left/right arrow keys or A/D keys.
Compilation
To compile the project, use the following command:

bash
Copy code
gcc -Wall -Werror -Wextra -pedantic ./src/*.c -IC:\MinGW\include\SDL2 -LC:\MinGW\lib -lmingw32 -lSDL2main -lSDL2 -lm -o maze
Once compiled, ensure that SDL2.dll is in the same folder as your executable, or that it is included in your system’s PATH. Then, run the program using ./maze (or maze.exe on Windows).


