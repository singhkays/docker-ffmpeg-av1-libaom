# docker-ffmpeg-av1-libaom
Adapted from https://hub.docker.com/r/offbytwo/ffmpeg 

Latest build of ffmpeg with latest build of AV1 built from libaom source @ https://aomedia.googlesource.com/aom/+/refs/heads/master. This also includes many common audio and video codecs, including HEVC/VP9/H.264.

Netflix's `libvmaf` support is also compiled in for running metrics on transcoded video.

## Usage

It's best to make another docker container and copy the contents of /opt/ffmpeg from this container to your new container. This will make for a much smaller image. But you can also run it directly with

```
docker run -it singhkays/ffmpeg-av1-libaom
```

