# How to add text with background to video using drawtext filter

```bash
ffmpeg -i in.mp4 -vf "drawtext=text='hola':box=1:boxborderw=5:boxcolor=black:x=10:y=10:fontsize=24:fontcolor=white" -c:a copy out.mp4
```

- `-i in.mp4` - input video file
- `-vf` - apply specific video filters
- `drawtext=` - drawtext filter options
- `text=` - text to draw
- `x=10` - horizontal position in pixels from top left corner
- `y=10` - vertical position in pixels from top left corner
- `fontsize` - size of the text to display
- `fontcolor` - color of the text
- `-c:a copy` - copy audio without converting
- `out.mp4` - resulting video file
- `box=1` - enabled background box for the text
- `boxborderw=5` - width of the background box border
- `boxcolor=` - text background color

group: drawtext


