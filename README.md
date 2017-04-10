## ofxCvColorImageAlpha

port of ofxCvColorImageAlpha to openFrameworks 0.9.3

https://forum.openframeworks.cc/t/opencv-ofxcvimage-how-to-load-an-external-file/2119

not all features have been tested


## Installation
copy files to ofOpofxOpenCv folder

add this line to ofxOpenCv.h file
```
#include "ofxCvColorImageAlpha.h"

## Usage
```
ofApp.h
ofxCvColorImageAlpha	alphaColorImg;
ofImage img;
```
ofApp.cpp
setup()
	img.load("fileName.png");
	alphaColorImg.allocate(img.getWidth(), img.getHeight());
	alphaColorImg.setFromPixels(img.getPixels());
	
draw()
	alphaColorImg.draw(0, 0);







