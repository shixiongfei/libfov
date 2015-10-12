# libfov #

## About ##

libfov is a C library for calculating fields of view and lighting on low resolution rasters, suitable for roguelike games. In that screenshot below, imagine that green dot is your character in a computer game, and as you walk around (move between tiles on the grid), you want to know which tiles you can see and which tiles you cannot. libfov calculates exactly that.

It can also be used to calculate which tiles are lit from a light source (the fov source doesn't have to be your eyesight, it can be a lightbulb). libfov supports beams, so you can use it to do nice directed lighting effects such as torch/flashlight lights.

libfov is fairly flexible in its design. It does not impose a map data structure on you. It operates via a couple of callbacks. It leaves enough room for you to decide what you want to do with the algorithm. You could conceivably use it in a real-time grid-based game with flickering multicoloured torches hanging off the walls, or you could use it behind the scenes to decide that a monster can see you, without displaying it on the screen.

## Screenshots ##

![http://libfov.googlecode.com/svn/wiki/screenshots/libfov-1.0.3-demo.png](http://libfov.googlecode.com/svn/wiki/screenshots/libfov-1.0.3-demo.png)

libfov 1.0.3 SDL Demo

## License ##

[MIT license](http://www.opensource.org/licenses/mit-license.php)

## Getting libfov ##

Get the latest version from [the download section](http://code.google.com/p/libfov/downloads/list).

```
tar xvzf libfov-x.y.z.tar.gz
cd libfov-x.y.z
./configure && make
```

From here, you can `sudo make install` to make libfov available on your system globally, but it's recommended that you either include fov.c and fov.h in your own build process, or use static linking to reduce the runtime dependencies of your code.

### FreeBSD/Ports ###

  * http://www.freebsdports.info/ports/games/libfov.html
  * http://www.freshports.org/games/libfov

## Using libfov ##

  * [API](http://libfov.sourceforge.net/api)
  * [FAQ](FAQ.md)
  * [IRC Channel](IRC.md)

## Projects Using libfov ##

[Opdur](http://www.netikka.net/joyr/obdur/index.html) A roguelike game.

![http://libfov.googlecode.com/svn/wiki/screenshots/obdur-screenshot-3.png](http://libfov.googlecode.com/svn/wiki/screenshots/obdur-screenshot-3.png)


---


[Torch](http://nornagon.net/darcsweb.cgi?r=torch;a=summary) A libfov tech demo for the NDS.

![http://libfov.googlecode.com/svn/wiki/screenshots/torch.png](http://libfov.googlecode.com/svn/wiki/screenshots/torch.png)
![http://libfov.googlecode.com/svn/wiki/screenshots/torch6.gif](http://libfov.googlecode.com/svn/wiki/screenshots/torch6.gif)


---


[hfov](http://nornagon.net/darcsweb.cgi?r=hfov;a=summary) Haskell bindings for libfov.


---


[Temple of Zum](http://sourceforge.net/projects/templeofzum/) A roguelike game.

![http://libfov.googlecode.com/svn/wiki/screenshots/toz-screenshot.jpg](http://libfov.googlecode.com/svn/wiki/screenshots/toz-screenshot.jpg)