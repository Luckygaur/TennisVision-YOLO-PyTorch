Here's your updated README section with the **requirements list properly aligned to the left** and the **training model links** embedded as hyperlinks under "Key Features":

---

# 🎾 TennisVision: Real-Time Tennis Match Analysis using YOLO & PyTorch  
TennisVision is a cutting-edge real-time video analysis system that leverages YOLO for robust object detection and PyTorch for deep learning-based model execution. Designed specifically for tennis analytics, it processes match footage to automatically detect and track players, the tennis ball, and court lines, while delivering precise, high-accuracy insights.

This intelligent system not only identifies every object on the court but also computes advanced metrics such as:
Player movement speed , Ball shot speed , Average speed and shot speed per player , Shot counts , Player trails.
With high-performance video processing, TennisVision offers a comprehensive performance analysis tool .

Ideal for coaches, analysts, and enthusiasts looking to study strategy, agility, and gameplay patterns.

## Sample Output Videos  
Here is a screenshot from one of the output videos:

![Screenshot](output_videos/screenshot.jpeg)

## 📌 Key Features  

### 🎯 Player & Ball Detection  
Detects and tracks tennis players and the ball using YOLOv8 and YOLOv5.  
🔗 [Trained YOLOv5 Model](https://drive.google.com/file/d/1UZwiG1jkWgce9lNhxJ2L0NVjX1vGM05U/view?usp=sharing)

### 🧠 Court Keypoint Extraction  
Uses a custom CNN to identify court lines and extract keypoints for spatial understanding.  
🔗 [Trained Tennis Court Key Point Model](https://drive.google.com/file/d/1QrTOF1ToQ4plsSZbkBs3zOLkVt3MBlta/view?usp=sharing)

### 📊 Match Analytics  
Calculates metrics like player speed, shot speed, court coverage, and shot counts.

### 📽️ Annotated Visual Output  
Draws bounding boxes, player trails, and court lines in real-time on output video.

### 🧮 Shot and Movement Heatmaps  
Visualizes player movements and ball landings to study player patterns and strategy.

---

## 🛠️ Tech Stack  

**Frameworks & Libraries:** PyTorch, OpenCV, NumPy, Matplotlib, Pandas  

**Models:**  
- YOLOv8: Player detection  
- YOLOv5: Tennis ball detection  
- Custom CNN: Court keypoint detection  
- Visualization: OpenCV overlay, heatmap generation

---

## 🚀 Getting Started  

### 📦 Installation  
```bash
git clone https://github.com/Luckygaur/TennisVision-YOLO-PyTorch.git  
cd TennisVision-YOLO-PyTorch  
pip install -r requirements.txt  
```

### 📹 Usage  
Add your match video(s) to the `input_videos/` folder.  

Run the analysis:  
```bash
python main.py  
```

Output videos with overlays will be saved in `output_videos/`.

---

## 📁 Project Structure  
```
TennisVision-YOLO-PyTorch/
├── analysis/              # Core analytics scripts
├── constants/             # Constant values used across modules
├── court_line_detector/   # CNN-based court keypoint extraction
├── input_videos/          # Folder for raw match input videos
├── output_videos/         # Annotated output videos
├── models/                # YOLO and CNN model files
├── runs/                  # YOLO detect outputs
├── utils/                 # Helper functions and utilities
├── main.py                # Entry point script
└── requirements.txt       # Project dependencies
```

## 📋 Requirements  

- python 3.8  
- ultralytics  
- pytorch  
- pandas  
- numpy  
- opencv

---

Let me know if you’d like badge icons, contribution guidelines, or auto-generated doc examples added next!
