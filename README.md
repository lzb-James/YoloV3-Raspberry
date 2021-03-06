# YOLOv3 Raspberry set configuration

This repository contains YOLOv3 configuration based on raspberry images. Trained weights can detect following items:
- ripe raspberry
- unripe/rotten rasberry
- petiole
- unknown items other than raspberry (dirt, leafs, ...)

## Prerequisites

Configuration is for Ultralytics YOLOv3 implementation which is based on Python nad TensorFlow.

It can be installed by cloning following repository:

```
git clone https://github.com/ultralytics/yolov3.git
```

## Repository content

### Training files

* CFG file (YOLOv3 configuration)
* DATA file (raspberry set info)
* Names file (class list)
* Labels

Images and prebuilt weights are not included into repository because of file size. Please contact author in order to acquire access to these files. Link to google drive https://drive.google.com/drive/folders/1n-O9RY-0Azd68JihvcZ0HH5e3IDELSGj?usp=sharing

#### Image detection

##### Good
![Upload](readme-images/detected-good.jpg)

##### Bad
![Upload](readme-images/detected-bad.jpg)

### Dockerized application

Besides training set repository contains dockerized application for image detection. Aplication contains upload form where user uploads image. Output is labeled image. User can select which weights will be used for detection. Available weights are:

* yolov3
* yolov3-spp
* yolov3-tiny
* raspberry

#### Example (yolov3 weights)

![Upload](readme-images/yolo-upload.png)
![Result](readme-images/yolo-result.png)

#### Example (raspberry weights)

![Upload](readme-images/yolo-upload2.png)
![Result](readme-images/yolo-result2.png)
