# SVG-to-Android-Adaptive-Icons-PNG
A script for convering SVG file to adaptive icons


## Installation

```
npm install svgexport -g
```

## Usage
Create three SVG file named as 
adaptive_icon_background
adaptive_icon_foreground
icon
following the android guideline, the background must be square and without any transparency the used part of the foreground must be 66.6% smaller than the background the image must share the same size but you must add padding.
For example for a background of 108*108 the foreground must be 108*108 but the icon inside must be 72*72 pixel.

### Linux
```
./SVGtoPNG.sh
```


### Windows
```
SVGtoPNG.bat
```
