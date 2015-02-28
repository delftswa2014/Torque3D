### Required libraries:
| Ubuntu           | Fedora                |
|------------------|-----------------------|
| build-essential  | automake kernel-devel |
| nasm             | nasm                  |
| xorg-dev         | xorg-x11-server-devel |
| ninja-build      | ninja-build           |
| gcc-multilib     | gcc                   |
| g++-multilib     | gcc-c++               |
| cmake            | cmake                 |
| cmake-qt-gui     | cmake-gui             |
| libogg-dev       | libogg-devel          |
| libxft-dev       | libXft-devel          |
| libx11-dev       | libX11-devel          |
| libxxf86vm-dev   | libXxf86vm-devel      |
| libopenal-dev    | openal-soft-devel     |
| libfreetype6-dev | freetype-devel        |
| libxcursor-dev   | libXcursor-devel      |
| libxinerama-dev  | libXinerama-devel     |
| libxi-dev        | libXi-devel           |
| libxrandr-dev    | libXrandr-devel       |
| libxss-dev       | libXScrnSaver         |
| libglu1-mesa-dev | mesa-libGLU-devel     |

### Installing with yum:
Binaries:  
`sudo yum install automake kernel-devel nasm xorg-x11-server-devel ninja-build gcc gcc-c++ cmake cmake-gui`  

Libraries:  
`sudo yum install libogg-devel libXft-devel libX11-devel libXxf86vm-devel openal-soft-devel freetype-devel libXcursor-devel libXinerama-devel libXi-devel libXrandr-devel libXScrnSaver mesa-libGLU-devel`

### Multiarch builds:
In order to ensure that both the `i386` and `x86_64` versions of the libraries are installed, add the `--setopt=multilib_policy=all` flag to your install command:  
`sudo yum install --setopt=multilib_policy=all libogg-devel libXft-devel libX11-devel libXxf86vm-devel openal-soft-devel freetype-devel libXcursor-devel libXinerama-devel libXi-devel libXrandr-devel libXScrnSaver mesa-libGLU-devel`
