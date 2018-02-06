# ReTouch

ReTouch is an OpenGL application that enables editing and retouching of images using depth-maps in 2.5D. The depth maps are generated by [Volume](http://volume.gl), a state of the art tool, that uses a CNN (Convolutional Neural Network) to predict depth-maps from 2D images . ReTouch uses these depth-maps to enable the addition of depth of field and color retouching for the foreground and background separately.
1. [Demo Video](https://www.youtube.com/watch?v=CAsy_jm85ZY)
1. [Features](#features)
1. [Installation](#installation)
1. [Dependencies](#dependencies)

![Editor](https://github.com/juniorxsound/ReTouch/blob/master/resources/editor.gif)

## Features

- #### Image and Depth-map viewer

![Viewer](https://github.com/juniorxsound/ReTouch/blob/master/resources/depthmap.gif)

- #### Depth of field - switchable between foreground and background

![Depth of Field](https://github.com/juniorxsound/ReTouch/blob/master/resources/dof.gif)

- #### Color retouching  - Coloring for foreground and background separately

![Color](https://github.com/juniorxsound/ReTouch/blob/master/resources/color.gif)

## Installation

To install start by forking the repo using ```--recursive``` flag, to clone submodules too. e.g
```
git clone https://github.com/juniorxsound/ReTouch --recursive
```
Once you have the repo cloned, make sure you have [CMake](https://cmake.org) installed. Create a directory titled ```build/``` in the root folder of the repo, ```cd``` into that folder and run
```
cmake ../
```
Once CMake finshes you can easily run 
```
make
``` 
to build a new executable and run it by calling ```./ReTouch``` in the build folder

## Dependencies
- [GLFW](https://github.com/glfw/glfw)
- [GLEW](https://github.com/nigels-com/glew)
- [Eigen](https://github.com/libigl/eigen)
- [nanogui](https://github.com/wjakob/nanogui)

> Tested on macOS (10.13.2) using CMake (3.10.0)

> ReTouch was developed under the advisement of Prof. [Ken Perlin](https://github.com/futurerealitylab) and Prof. [Daniele Panozzo](https://github.com/danielepanozzo) @ NYU, Special thanks to [Shirin Anlen](http://shirin.works)
