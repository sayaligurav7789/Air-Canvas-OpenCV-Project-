# ✨ Air-Canvas Project  
### *Draw in the Air Using Computer Vision & OpenCV!*  

Ever imagined drawing in the air **without touching anything**?  
The Air-Canvas Project brings that imagination to life! Using **OpenCV**, **Python**, and a colored marker, you can draw virtually in real time — just by waving your hand in front of the camera.

---

## 🚀 Features  
- 🎨 **Hands-Free Drawing** — Create art using a colored marker in mid-air.  
- 🤖 **Computer Vision Powered** — Uses OpenCV for color detection, contour tracking, and mask refinement.  
- 🖼️ **Dual Window View** — Live tracking + virtual paint window.  
- 🌈 **Multiple Ink Colors** — Switch colors using on-screen buttons.  
- ⚙️ **Trackbars for Calibration** — Fine-tune HSV ranges precisely.  
- 📚 **Fun + Educational** — Great for learning real-time image processing.

---

## 🧠 How It Works  

### 1️⃣ Frame Capture  
- Capture webcam video frames.  
- Convert each frame to **HSV color space** for better color segmentation.

### 2️⃣ Color Detection  
- Apply HSV thresholding to isolate the chosen marker color.  
- Tune thresholds using **trackbars** for accurate detection.

### 3️⃣ Mask Refinement  
- **Erosion:** Removes noise.  
- **Dilation:** Restores correct marker shape.  
These steps make the mask clean and stable.

### 4️⃣ Contour Detection  
- Find contours from the mask.  
- Identify the **largest contour** (marker).  
- Calculate its **center point** — this becomes the drawing tip.

### 5️⃣ Point Tracking  
- Store the center positions across frames.  
- These points form the **path** of your drawing.

### 6️⃣ Drawing on the Canvas  
- Draw lines between consecutive points on:  
  - The **live video feed**  
  - The **virtual canvas window**

### 7️⃣ Display  
The app shows:  
- 🖼️ **Paint Window**  
- 🖤 **Mask Window**  
- 🌈 **Color Detection Window**  
- 🎯 **Tracking Window**

---

## 🛠️ Requirements  

- Python 3  
- OpenCV  
- NumPy  
- Webcam  

Install dependencies:  
```bash
pip install opencv-python numpy
```
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
