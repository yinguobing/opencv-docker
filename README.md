# opencv-docker
Dockerfiles for OpenCV build.

## Build FFMPEG
```bash
docker build -t yinguobing/ffmpeg:4.3.3 -f ffmpeg .
```

## Build FFMPEG with CUDA support
```bash
docker build -t yinguobing/ffmpeg:4.3.3-cuda-11.3.1 -f ffmpeg-cuda .
```
