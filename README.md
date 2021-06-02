# Distance_Birdview
Using python, deep learning and computer vision to monitor social distancing.

## Install required packages
The provided requirements.txt file can be used to install all the required packages. Use the following command

```

pip install –r requirements.txt
```


## Run the project
```
python main.py --videopath "vid_short.mp4"
```

Running main.py will open a window of the first frame in the video. At this point the code expects the user to mark 6 points by clicking appropriate positions on the frame.

#### First 4 points:
The first 4 among the 6 required points are used to mark the Region of Interest (ROI) where you want to monitor. Moreover, the lines marked by these points should be parallel lines in real world as seen from above. For example these lines could be the curbs of the road.
These 4 points need to be provided in a pre-defined order which is following.

* __Point1 (bl)__: Bottom left
* __Point2 (br)__: Bottom right
* __Point3 (tl)__: Top left
* __Point4 (tr)__: Top right



#### Last 2 points:
The last two points are used to mark two points 6 feet apart in the region of interest. For example this could be a person's height (easier to mark on the frame)



A detailed article on the working of this project can be found [here](https://medium.com/@aqeel.anwar/monitoring-social-distancing-using-ai-c5b81da44c9f)

__Idea credits: LandingAI__
