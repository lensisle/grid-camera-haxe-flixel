# HaxeFlixel GridCamera

HaxeFlixel GridCamera is a tiny class for HaxeFlixel that emulates the screen transition effect of the first The Legend of Zelda game.

Example: 

![The Legend of Zelda](https://raw.github.com/camiloei/HaxeFlixel-GridCamera/master/image/tloz.gif)

### Installation
Just include this class in your haxeflixel project.

### Usage

Using this class is very simple. First, initialize:

```haxe
var gridCamera = new GridCamera(
                        actor:FlxSprite,            
                        mapWidthInTiles:Int,
                        mapHeightInTiles:Int, 
                        tileSize:Int, 
                        camera:FlxCamera, 
                        currentGridX:Int=0, 
                        currentGridY:Int=0,
                        transitionTime:Float=1.5
                  );
```
* **actor**: the object that interacts with the camera
* **mapWidthInTiles**: number of width tiles (total) of your map 
* **mapHeightInTiles**:  number of height tiles (total) of your map
* **tileSize**: the size of your tiles.
* **camera**: the camera object (the camera where your map and actor are rendered).
* **currentGridX**: the starting grid x of your actor (default is 0)
* **currentGridY**: the starting grid y of your actor (default is 0)
* **transitionTime**: the time that takes passing from one screen to other (default is 1.5 seconds)

Then, you have to set the camera:

```haxe
gridCamera.set();
```

This method set the camera bounds and initialize coordinate variables.

And finally, you have to update the camera (in your update method):

```haxe
gridCamera.update();
```

result:

![Example](https://github.com/camiloei/HaxeFlixel-GridCamera/raw/master/image/example.gif)

### Thanks for visiting!

Feel free to use this class whatever you want whenever you want.

You can tweet me at @camiloei if you have questions.
