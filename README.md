# opencv-docker
Dockerfiles for OpenCV build.

## FFMPEG
OpenCV depends on FFMPEG as it's video io backend.

### FFMPEG development
Build a FFMPEG development image without any hardware accelerators.

```bash
docker build -t yinguobing/ffmpeg:4.3.3-devel-ubuntu22.04 -f ffmpeg-devel .
```

### FFMPEG runtime
Build a FFMPEG runtime image without any hardware accelerators. This will 
provide a minimal sized image.

```bash
docker build -t yinguobing/ffmpeg:4.3.3-runtime-ubuntu22.04 -f ffmpeg-runtime .
```

### FFMPEG with CUDA development
Build a FFMPEG development image with NVIDIA hardware accelerators. This image 
will be usefull if you want to build other libraries on top of NVIDIA accelerated 
FFMPEG.

```bash
docker build -t yinguobing/ffmpeg:4.3.3-cuda_11.8.0-devel-ubuntu22.04 -f ffmpeg-cuda-devel .
```

### FFMPEG with CUDA runtime
Build a FFMPEG runtime image with NVIDIA hardware accelerators. This image could 
be used as a deployment base image for your applications.

```bash
docker build -t yinguobing/ffmpeg:4.3.3-cuda_11.8.0-runtime-ubuntu22.04 -f ffmpeg-cuda-runtime .
```

## OpenCV

### OpenCV development
Build an OpenCV development image. This image will be useful if you want to 
build other libs based on OpenCV libs. Note there is no hardware acceleration 
available in this image.

```bash
docker build -t yinguobing/opencv:4.5.4-devel-ubuntu22.04 -f opencv-devel .
```

### OpenCV runtime
Build an OpenCV runtime image. This image could be used as a deployment base 
image for your applications.

```bash
docker build -t yinguobing/opencv:4.5.4-runtime-ubuntu22.04 -f opencv-runtime .
```

### OpenCV with CUDA development
Build an OpenCV development image with NVIDIA CUDA support. This image will be 
useful if you want to build other libs based on OpenCV libs.

```bash
docker build -t yinguobing/opencv:4.5.4-cuda_11.8.0-devel-ubuntu22.04 -f opencv-cuda-devel .
```

### OpenCV with CUDA runtime
Build an OpenCV runtime image with NVIDIA CUDA support. This image could be used 
as a deployment base image for your applications.

```bash
docker build -t yinguobing/opencv:4.5.4-cuda_11.8.0-runtime-ubuntu22.04 -f opencv-cuda-runtime .
```

### OpenCV with CUDA development
Build an OpenCV development image with NVIDIA CUDA support. This image will be 
useful if you want to build other libs based on OpenCV libs.

```bash
docker build -t yinguobing/opencv:4.5.4-cuda_11.8.0-devel-ubuntu22.04 -f opencv-cuda-devel .
```

### OpenCV with RUST development
Build an OpenCV development image with RUST language support.

```bash
docker build -t yinguobing/opencv:4.5.4-devel-rust-ubuntu22.04 -f opencv-rust-devel .

```