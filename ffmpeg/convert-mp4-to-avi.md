# Convert mp4 to avi

### Since `avi` and `mp4` are containers, not codecs, we simply copy video/audio streams:

```bash
ffmpeg -i in.mp4 -c:v copy -c:a copy out.avi
```

- `ffmpeg` - name of the package to install
- `-i in.mp4` - input video file
- `-c:v copy` - just copy video stream from input to output
- `-c:a copy` - just copy audio stream from input to output
- `out.avi` - resulting file

group: avi


