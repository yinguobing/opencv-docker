# opencv-docker
Dockerfiles for OpenCV build.

## Build FFMPEG runtime image
```bash
docker build -t yinguobing/ffmpeg:4.3.3-runtime-ubuntu20.04 -f ffmpeg .
```

## Build FFMPEG with CUDA development image
```bash
docker build -t yinguobing/ffmpeg:4.3.3-cuda_11.3.1-devel-ubuntu20.04 -f ffmpeg-cuda-devel .
```

## Build FFMPEG with CUDA runtime image
```bash
docker build -t yinguobing/ffmpeg:4.3.3-cuda_11.3.1-runtime-ubuntu20.04 -f ffmpeg-cuda-runtime .
```