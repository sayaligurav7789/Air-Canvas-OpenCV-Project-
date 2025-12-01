# Air-Canvas Project
#### A Computer Vision Project with OpenCV

Bring your imagination to life by drawing in the air! This project allows you to create a virtual drawing on a canvas using a colored marker, tracked in real-time using OpenCV and Python. Here's a detailed breakdown of how it works:

#### Key Highlights
Hands-Free Drawing: Draw virtually by waving a colored marker in front of a camera.
Computer Vision at Work: Leverages OpenCV techniques for color detection, tracking, and contour analysis.
User-Friendly Interface: Includes a virtual canvas with color options for easy interaction.
Educational and Fun: Learn fundamental image processing concepts while building an interactive project.
#### How It Works: Step-by-Step
##### 1. Frame Capture
Capture video frames from your webcam.
Convert frames to HSV color space, which simplifies color detection.
##### 2. Color Detection
Detect the colored marker by isolating its color using HSV thresholds.
Use trackbars to fine-tune the color range for precision.
#### 3. Mask Refinement
Apply morphological operations like:
Erosion: Removes noise from the mask.
Dilation: Enhances the cleaned mask to restore the marker's shape.
#### 4. Contour Detection
Identify contours in the mask to locate the largest one, corresponding to the marker.
Calculate the center of the contour, which represents the tip of the marker.
#### 5. Point Tracking
Store the center points of the marker in arrays for each successive frame.
These points form the path of the marker’s movement.
#### 6. Drawing on the Canvas
Render lines between the stored points on both:
The live video feed.
A separate virtual canvas.
#### 7. Display
Show the processed video feed ("Tracking") and the canvas ("Paint") simultaneously.
#### Features
- Real-Time Tracking: Smoothly tracks the marker’s movement with minimal lag.
- Multiple Colors: Switch between ink colors by interacting with on-screen buttons.
- Interactive Canvas: Enables users to view their drawings alongside the live feed.
#### Requirements
- Python 3
- OpenCV
- Numpy
#### Advantages of the Project
- Practical Learning: Master OpenCV techniques like color masking, contour tracking, and morphological operations.
- Interactive and Fun: Explore the potential of computer vision in a creative and enjoyable way.
- Real-World Applications: Expand these concepts for gesture recognition, augmented reality, or interactive displays.

### Snapshots:
#### Paint Window:    
<img width="481" height="373" alt="image" src="https://github.com/user-attachments/assets/3349bdc9-5d41-4491-910b-0a57005ef0c1" />

---

#### Mask Window:
<img width="474" height="366" alt="image" src="https://github.com/user-attachments/assets/c274bfd0-c1e8-4222-8ef8-c81940942d8c" />

---

#### Colour Detections Window:
<img width="940" height="266" alt="image" src="https://github.com/user-attachments/assets/dd46d747-b00f-4551-a8d8-36e24272fec1" />

----

#### Tracking Window:
<img width="1069" height="481" alt="image" src="https://github.com/user-attachments/assets/ccb65e28-d501-4bd5-8206-760a220e29b4" />
