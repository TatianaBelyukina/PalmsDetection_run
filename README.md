# PalmsDetection_run
## Overview

This project is designed to detect palm trees on map screenshots. The detection results are saved as annotations in the form of bounding boxes for each object found in the images. These annotations are stored in .txt files in the YOLO format.

## How to Use
You only need to run the script inter.py to execute the detection. In this file, you'll find a command that looks like the following:

'''bash !python detect.py --weights /Users/tetiana/Documents/python_files/yolov5/yolov5-master/runs/train/yolov5_custom/weights/last.pt --img 640 --conf 0.4 --source /Users/tetiana/Documents/python_files/Palm-Counting-349images/test_maps_ph --save-txt --save-conf'''

##Steps:

1. Update the file path: Change the path after the --source argument to point to the directory where your map screenshots are stored. This will ensure the detection runs on your files.

2. Run the script: Execute inter.py to run the detection.

3. View Results:

  After running the script, the detection results will be saved in the runs/detect/exp/labels folder.
  The .txt files in this folder contain the bounding box annotations for each detected object in your images.
  
## Data Format

The .txt files generated for each image contain lines of information representing the bounding boxes of detected objects. Each line corresponds to a detected object and follows this format:

class x_center y_center width height confidence



