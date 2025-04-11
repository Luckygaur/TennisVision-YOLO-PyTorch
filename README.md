🎾 TennisVision: Real-Time Tennis Match Analysis using YOLO & PyTorch
TennisVision is a real-time video analysis system built using YOLO for object detection and PyTorch for deep learning. It processes match footage to detect players and the ball, identify court regions, and derive insightful statistics for performance evaluation.

📌 Key Features
🎯 Player & Ball Detection
Detects and tracks tennis players and the ball using YOLOv8 and YOLOv5.

Trained YOLOv5 Model

🧠 Court Keypoint Extraction
Uses a custom CNN to identify court lines and extract keypoints for spatial understanding.

Trained Tennis Court Key Point Model

📊 Match Analytics
Calculates metrics like player speed, shot speed, court coverage, and shot counts.

📽️ Annotated Visual Output
Draws bounding boxes, player trails, and court lines in real-time on output video.

🧮 Shot and Movement Heatmaps
Visualizes player movements and ball landings to study player patterns and strategy.

🛠️ Tech Stack
Frameworks & Libraries: PyTorch, OpenCV, NumPy, Matplotlib, Pandas

Models:

YOLOv8: Player detection

YOLOv5: Tennis ball detection

Custom CNN: Court keypoint detection

Visualization: OpenCV overlay, heatmap generation

🚀 Getting Started
📦 Installation
bash
Copy
Edit
git clone https://github.com/Luckygaur/TennisVision-YOLO-PyTorch.git  
cd TennisVision-YOLO-PyTorch  
pip install -r requirements.txt  
📹 Usage
Add your match video(s) to the input_videos/ folder.

Run the analysis:

bash
Copy
Edit
python main.py  
Output videos with overlays will be saved in output_videos/.

📁 Project Structure
graphql
Copy
Edit
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
🧪 Sample Output Preview
Insert sample screenshots or video gif of detection + stats overlay here

## Output Videos
Here is a screenshot from one of the output videos:

![Screenshot](output_videos/screenshot.jpeg)

## Requirements
* python3.8
* ultralytics
* pytroch
* pandas
* numpy 
* opencv
