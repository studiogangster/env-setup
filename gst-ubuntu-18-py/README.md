```bash
docker build -t gstreamer-python:latest .
```

```bash
xhost +local:  # to enable GUI

sudo docker run --name gstreamer-python -it \
-e DISPLAY=$DISPLAY
-v /tmp/.X11-unix/:/tmp/.X11-unix \
gstreamer-python:latest
```
