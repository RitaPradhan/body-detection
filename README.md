

#  Full Body Detection Using OpenCV

This project detects **human full bodies** in a video using **Haar Cascade Classifier** with OpenCV.

The program processes a video file provided by the user and draws bounding boxes around detected bodies in real time.

---

##  Overview

The system uses a pre-trained **Haar Cascade Full Body XML model** to identify human bodies frame-by-frame from a video input.

---

##  Features

* Full body detection in video files
* Uses Haar Cascade classifier
* Real-time bounding box visualization
* Simple user input for video path

---

##  Technologies Used

* Python
* OpenCV

---

##  Requirements

* Python 3.7+
* OpenCV
* Haar Cascade Full Body XML file

---

##  Installation

```bash
pip install opencv-python
```

Download the Haar Cascade file:
`haarcascade_fullbody.xml`

---

##  Usage

1. Update the Haar Cascade file path in the code:

```python
body_cascade = cv2.CascadeClassifier("path/to/haarcascade_fullbody.xml")
```

2. Run the script:

```bash
python full_body_detection.py
```

3. Enter the video file path when prompted.

4. Press **`q`** to quit.

---

## How It Works

1. Loads Haar Cascade classifier
2. Reads video frames
3. Converts frames to grayscale
4. Detects full bodies
5. Draws bounding boxes around detections

---

##  Key Parameters

| Parameter          | Description                  |
| ------------------ | ---------------------------- |
| `detectMultiScale` | Detects objects in the frame |
| `1.1`              | Scale factor                 |
| `3`                | Minimum neighbors            |

---

##  Limitations

* Works best with clear, upright human bodies
* Sensitive to lighting and video quality
* Less accurate than deep learning models
* May detect false positives

---

##  Author

**Rita Pradhan**

---

##  License

This project is for **educational purposes only**.

---


