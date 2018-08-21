# Shader fun

*Session by Marc.*
*Written by [@NarigoDF](https://twitter.com/NarigoDF).*

We've played around with Marcs [shader-playground](https://github.com/SheepFromHeaven/shader-playground) repository and
later had a look at [shadertoy](https://www.shadertoy.com/). [The Eye demo](https://www.shadertoy.com/view/MsKBDG) is 
still giving me nightmares as many vector values were more or less randomly edited, resulting in extremely strange 
effects.

After playing with [shader-playground](https://github.com/SheepFromHeaven/shader-playground) during the session, we 
decided to add a live editor on the page. You can now 
[code directly on the GitHub page](https://sheepfromheaven.github.io/shader-playground) and play around with the 
images.

Try for example switching channels by using this code:

```
newPixel[CHANNEL.RED] = currentPixel[CHANNEL.GREEN];
newPixel[CHANNEL.GREEN] = currentPixel[CHANNEL.BLUE];
newPixel[CHANNEL.BLUE] = currentPixel[CHANNEL.RED];
newPixel[CHANNEL.ALPHA] = currentPixel[CHANNEL.ALPHA];
```
