The pitches in the games in the Kick Off Series are stored on the floppies using a technique called tiling. Two files are used for each pitch: A bitmap which contains a number of 16 x 16 pixel tiles and a tilemap which holds indices into the bitmap. The size of the maps are 80 x 96 tiles and consequently the size of a full pitch is 1280 x 1536 pixels.

In openkickoff it is nearly the same except that bitmap has been converted from IFF amiga format to PNG and tilemap has been converted from binary to TMX file, which is a XML description of the tilemap used by TilED map editor.

TilED is a generic tool for tile map editing and can be found at: http://mapeditor.org/

With [Slick](http://slick.cokeandcode.com/) library, you can use the Class [TiledMap](http://slick.cokeandcode.com/javadoc/org/newdawn/slick/tiled/TiledMap.html) which is able to create a new tile map based on a given TMX file.

openkickoff version include the following four pitches

  * Normal
  * Wet
  * Soggy
  * Plastic

![http://ko-gathering.com/wiki/images/c/c5/Ko2_pitch_normal_snapshot.png](http://ko-gathering.com/wiki/images/c/c5/Ko2_pitch_normal_snapshot.png)
> Normal Pitch

![http://ko-gathering.com/wiki/images/1/12/Ko2_pitch_wet_snapshot.png](http://ko-gathering.com/wiki/images/1/12/Ko2_pitch_wet_snapshot.png)
> Wet Pitch

![http://ko-gathering.com/wiki/images/8/82/Ko2_pitch_soggy_snapshot.png](http://ko-gathering.com/wiki/images/8/82/Ko2_pitch_soggy_snapshot.png)
> Soggy Pitch

![http://ko-gathering.com/wiki/images/b/be/Ko2_pitch_artificial_snapshot.png](http://ko-gathering.com/wiki/images/b/be/Ko2_pitch_artificial_snapshot.png)
> Plastic Pitch

More infos on [KORPS](http://ko-gathering.com/wiki/index.php?title=Pitches) (Kick Off Research Project Society)