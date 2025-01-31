# 🎨 Real-Time Color Detection using OpenCV

## 📌 Overview
This project implements real-time color detection using OpenCV and Python. It allows users to dynamically adjust HSV color thresholds using trackbars and detect objects of a specific color range from a webcam feed.

## 🛠 Features
- 🎥 Captures real-time video feed from a webcam
- 🎚 Adjustable HSV thresholds via interactive trackbars
- 🎭 Creates a binary mask to isolate specific colors
- 🔍 Detects contours and convex hulls of detected objects
- 🖼 Displays processed output including masked, thresholded, and filtered images

## 📂 Installation
```bash
pip install opencv-python numpy
```

## 🚀 Usage
Run the script to start real-time color detection:
```bash
python main.py
```

Press `Esc` to exit the application.

## 🖼 Output

![image](https://github.com/user-attachments/assets/aae94ce2-e4a8-4e92-9e1a-dcd612ce8496)

- **Masked Output**: Displays the isolated color region.
- **Filtered Output**: Shows the result after applying the mask.
- **Final Result**: Highlights detected contours and convex hulls.

## 📜 Explanation
1. **Reading Camera Input** 🎥
   - Captures video feed from the webcam using `cv2.VideoCapture(0)`.
2. **Creating Trackbars** 🎚
   - Adjustable HSV threshold values to filter out specific colors.
3. **Applying Color Masking** 🎭
   - Uses `cv2.inRange` to create a mask for the specified color range.
4. **Processing and Contour Detection** 🔍
   - Applies thresholding and dilation to enhance detected objects.
   - Finds contours using `cv2.findContours`.
5. **Drawing Contours and Convex Hulls** 🖌
   - Draws detected contours and convex hulls around objects.

## 📬 Contact
For any queries or improvements, feel free to reach out! 😊

