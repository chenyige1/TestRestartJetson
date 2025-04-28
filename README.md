# TestRestartJetson

jetson orin nx super running restart problems

#### At present, the program will freeze completely after running on Jetson orin nx super (deepstream7.1 jetpack6.1) for 1-14 hours, and then restart the computer after a period of time

you can try to adjust the piplines and the plugins properties of file:
```
./aiStream/gtyStream/stream_task.py
```
the configFiles all under the path:
```
./aiStream/config.ini
./aiStream/gtyStream/configFiles/...
```
the video using Ethernet local video loop streaming, for example:
```
ffmpeg -re -stream_loop -1 -i 6long.mp4 -c copy -f rtsp rtsp://127.0.0.1:8554/stream4
```
the local marathon video is so big (400+MB) that cannot upload, so you can find a runner video with bib digital, and config bib info in ./aiStream/config.ini file