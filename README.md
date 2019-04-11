# SVG to Android Adaptive Icons PNG
A script for convering SVG file to adaptive icons


## Installation

```
npm install svgexport -g
```

## Usage
Create three SVG file named as 

* adaptive_icon_background
* adaptive_icon_foreground
* icon

following the android guideline, the background must be square and without any transparency the used part of the foreground must be 66.6% smaller than the background the image must share the same size but you must add padding.

For example for a background of 108\*108 the foreground must be 108\*108 but the icon inside must be 72\*72 pixel.

### Linux
```
./SVGtoPNG.sh
```


### Windows
```
SVGtoPNG.bat
```

## Import in Android Studio
After importing in android studio remember to define a folder named *minmap-any-dpi-v26*
with a single file inside named *launcher_icon.xml* with the following code

```
<?xml version="1.0" encoding="utf-8"?>
  <adaptive-icon xmlns:android="http://schemas.android.com/apk/res/android">
  <background android:drawable="@drawable/ic_launcher_background"/>
  <foreground android:drawable="@drawable/ic_launcher_foreground"/>
</adaptive-icon>
```
