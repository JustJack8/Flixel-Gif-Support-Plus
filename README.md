# About
This is my own little fork of [GrowtopiaFli's](https://github.com/GrowtopiaFli) [Flixel Gif Code](https://github.com/GrowtopiaFli/openfl-haxeflixel-gif-code) which made it into a haxelib and organized folders and what not
# Instructions
First, git the haxelib by pasting this command into the cmd or powershell.
```
haxelib git flixel-gif-plus https://github.com/JustJack8/Flixel-Gif-Support-Plus
```

You also have to install yagp
```
haxelib install yagp
```

Next, in your Project.XML add this line of code under your libaries
```
<haxelib name="flixel-gif-plus"/>
```

After that, import the FlxWindowModifier from this repository to yours.
```
import gif.FlxGifSprite;
```

#Example use(s)
```
var gif:FlxGifSprite;
gif = new FlxGifSprite('AssetPath', X, Y, Width, Height);
add(gif);
```

Keep in mind, this also extends to an FlxSprite so all the functions from there also apply to here (ScreenCenter, Alpha, etc)

## Credits:
* [JustJack] (https://twitter.com/Just_Jack6)
* [GrowtopiaFli] (https://github.com/GrowtopiaFli) - Made the orginal support
* [Yanrishatum] (https://github.com/Yanrishatum) - Made yagp