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
![img.png](img.png)