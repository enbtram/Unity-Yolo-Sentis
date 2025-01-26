---
library_name: unity-sentis
pipeline_tag: object-detection
---
# YOLOv8n validated for Unity Sentis (Version 1.4.0-pre.3*)
*Version 1.3.0 sentis files are not compatible with 1.4.0 and will need to be recreated/downloaded

[YOLOv8n](https://docs.ultralytics.com/models/yolov8/) is a real-time multi-object recognition model confirmed to run in Unity 2023.

## How to Use
First get the package `com.unity.sentis` from the package manager.
You will also need the Unity UI package.

* Create a new scene in Unity 2023.
* Install `com.unity.sentis` version `1.4.0-pre.3` from the package manager
* Add the c# script to the Main Camera.
* Create a Raw Image in the scene and link it as the `displayImage`
* Drag the yolov8n.sentis file into the model asset field
* Drag the classes.txt on to the labelAssets field
* Put a video file in the Assets/StreamingAssets folder and set the name of videoName to the filename in the script
* Set the fields for the bounding box texture sprite (you can [create your own one](https://docs.unity3d.com/Manual/9SliceSprites.html) using a transparent texture or use an inbuilt one) and the font


## Preview
If working correctly you should see something like this:

![preview](preview.png)

## Information
The NMS selection will be improved in later versions of Sentis. Currently uses singular-class approach.

## Unity Sentis
Unity Sentis is the inference engine that runs in Unity 3D. More information can be found at [here](https://unity.com/products/sentis)

## License
The YOLO models use the GPLv3 license.