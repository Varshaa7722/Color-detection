# Color Detection using OpenCV

This project enables real-time color detection using OpenCV. It captures video from your webcam, converts each frame to the HSV color space, and applies color masks to detect specific colors like red, green, blue, and yellow. The detected color regions are highlighted in the video feed.

## Requirements
1. Python 

2. OpenCV

3. NumPy
   
4. Pillow


### Working Principle:
1. Capture Video:

The script uses OpenCV to access the webcam and read video frames.

2. Convert to HSV:

Each frame is converted from BGR to HSV color space, which is more suitable for color detection.

3. Define Color Ranges:

For each target color, HSV lower and upper bounds are defined. For example, red color detection may require two ranges due to HSV hue wrap-around.

4. Create Masks:

Using cv2.inRange(), masks are created for each color range to isolate the desired color regions.

5. Apply Masks:

The masks are applied to the original frame to extract and display the detected color regions.

#### NOTE: This project detects yellow objects as of now 
