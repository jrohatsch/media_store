generated gifs with command:

```
ffmpeg -i input.mp4 -ss 00:00:10 -to 00:00:15 -vf "fps=15,split[s0][s1];[s0]palettegen[p];[s1][p]paletteuse" -loop 0 output.gif
```