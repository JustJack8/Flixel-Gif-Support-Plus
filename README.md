# About
This is my own little fork of [GrowtopiaFli's](https://github.com/GrowtopiaFli) [Flixel Gif Code](https://github.com/GrowtopiaFli/openfl-haxeflixel-gif-code) which made it into a haxelib and organized folders and what not
# Instructions (General)
First, git the haxelib by pasting this command into the cmd or powershell.
```
haxelib git flixel-gif-plus https://github.com/JustJack8/Flixel-Gif-Support-Plus
```

You also have to install yagp
```
haxelib install yagp
```

Next, in your Project.XML add these lines of code under your libaries
```xml
<haxelib name="flixel-gif-plus"/>
<haxelib name="yagp"/>
```

After that, import the FlxGifSprite from this repository to yours.
```haxe
import gif.FlxGifSprite;
```

# Example use
```haxe
var gif:FlxGifSprite;
gif = new FlxGifSprite('AssetPath', X, Y, Width, Height);
add(gif);
```

# For Friday Night Funkin

Create a folder called `gifs` in your `assets/preload` folder.

Next, Put this along with the other inline functions in `Paths.hx`
```haxe
inline static public function gif(key:String)
{
   return 'assets/gifs/$key.gif';
}
```

# Example use For FNF
```haxe
var gif:FlxGifSprite;
gif = new FlxGifSprite(Paths.gif('ImagePath'), X, Y, Width, Height);
add(gif);
```
## Keep in mind, this also extends to an FlxSprite so all the functions from there also apply to here (ScreenCenter, Alpha, etc)

## Credits:
* [JustJack] (https://twitter.com/Just_Jack6)
* [GrowtopiaFli] (https://github.com/GrowtopiaFli) - Made the orginal support
* [Yanrishatum] (https://github.com/Yanrishatum) - Made yagp