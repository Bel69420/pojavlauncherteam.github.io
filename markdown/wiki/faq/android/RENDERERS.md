# Renderers 
Minecraft runs on OpenGL, and mobile devices generally only support OpenGL ES (GLES). And since Minecraft won't run on GLES, we have to use renderers as compatibility layers between OpenGL ES and OpenGL.
> All of the following renderers were tested using the same environment; Minecraft 1.21.1 with Optifine, 8 chunks, running on a Snapdragon 778g at 80% resolution scale, with Fast graphics and smooth lighting.

## Holy GL4ES
- Optimized for performance, Holy GL4ES is the default renderer in PojavLauncher and should be used in almost all scenrarios. 
- Supports OpenGL 2.1 and has shader converting capabilities, thus makes up for about 1/8 of the OpenGL 3.x standard.
- Works on all versions of vanilla Minecraft.
### A screenshot of Holy GL4ES running Minecraft 1.21.1
![holygl4es](https://raw.githubusercontent.com/whal-whales/random-imgs-repo-for-stuff/refs/heads/main/2024-09-22_12.32.23.png)

### A screenshot of ANGLE running Minecraft 1.21.1
![angle](https://raw.githubusercontent.com/whal-whales/random-imgs-repo-for-stuff/refs/heads/main/Screenshot_20240922_124430_PojavLauncher%20(Minecraft%20Java%20Edition%20for%20Android).jpg)

## Zink
- Mid. It's only useful for mods that don't run due to missing OpenGL extensions and for running shaders.
- Supports OpenGL 4.5 on Adreno GPUs with Turnip, and OpenGL 3.1/3.2(*) on Mali GPUs. Adreno GPUs without Turnip
**will** face crashes when using Zink.
- Works on all vanilla versions of Minecraft.

### A screenshot of Zink running Minecraft 1.21.1
![Zink](https://raw.githubusercontent.com/whal-whales/random-imgs-repo-for-stuff/refs/heads/main/2024-09-22_12.38.14.png)

## MobileGlues 
- Fast/mid, runs on OpenGLES 3.x and used for mods compatibility and shaders.
- Supports partial OpenGL 4.x
- Only works on versions 1.17+
- In video and renderers settings, there is an extra renderer option where you can adjust the renderer's configuration (eg. Enable angle as es driver and more.)

### A screenshot of MobileGlues running on Minecraft 1.21.4
(coming soon)
