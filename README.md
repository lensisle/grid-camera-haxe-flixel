# HaxeFlixel GridCamera

HaxeFlixel GridCamera is a tiny class for HaxeFlixel that emulates the screen transition effect of the The Legend of Zelda 2D.

Example: 

![The Legend of Zelda](https://raw.github.com/camiloei/HaxeFlixel-GridCamera/master/image/tloz.gif)

### Installation
just include this class in your haxeflixel project.

### Usage

using this class is very simple. First, initialize:

```sh
var gridCamera:GridCamera = new GridCamera(
                                actor:FlxSprite,            
                                mapWidthInTiles:Int,
                                mapHeightInTiles:Int, 
                                tileSize:Int, 
                                cameraWidth:Int, 
                                cameraHeight:Int, 
                                currentGridX:Int=0, 
                                currentGridY:Int=0,
                                transitionTime:Float=1.5
                        );
```
* **actor**: the object interacts with the camera
* **mapWidthInTiles**: number of width tiles (total) of your map 
* **mapHeightInTiles**:  number of height tiles (total) of your map
* **tileSize**: the size of your tiles.
* **cameraWidth**: the current width of your camera. (frecuently is the width of the FlxG.camera object)
* **cameraHeight**: the current height of your camera. (frecuently is the height of the FlxG.camera object)
* **currentGridX**: the starting grid x of your actor (default is 0)
* **currentGridY**: the starting grid y of your actor (default is 0)
* **transitionTime**: the time that takes passing from one screen to other (default is 1.5)

then, you have to set the camera:

```sh
gridCamera.set();
```

this method set the camera bounds and initialize coordinate variables.

and finally, you have to update the camera (in your update method):

```sh
gridCamera.update();
```

result:

![Example](https://github.com/camiloei/HaxeFlixel-GridCamera/raw/master/image/example.gif)

### Thanks for visiting!

Feel free to use this class whatever you want whenever you want.

you can tweet me at @camiloei if you have questions.
