# Drone live object recognition
Get live object detection from you personal drone


I'm using DJI mini2

## Set Up
1. Download [Local RTMP Server](https://github.com/sallar/mac-local-rtmp-server)
2. run `ifconfig | grep "inet "` in terminal to get your ip address
3. put the link of format `rtmp://<IP ADDRESS>/live/<ANYTHING>` to the drone's RTMP transmission settings and start the transmission. Save this link for later
4. run 
```
git clone https://github.com/ultralytics/yolov5
cd yolov5
python3 detect.py --source 'rtmp://<IP ADDRESS>/live/<ANYTHING>'
```
Wathch the [example](https://youtu.be/Q4YGRJSYXKE) 
