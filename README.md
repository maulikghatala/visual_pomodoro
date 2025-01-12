# 🍅 Visual Pomodoro Assistant

A professional desktop application that combines a Pomodoro timer with computer vision to ensure you remain at your desk during work sessions. Features modern UI, real-time human detection, audio alerts, and comprehensive session tracking.

![Python](https://img.shields.io/badge/Python-3.13+-blue.svg)
![OpenCV](https://img.shields.io/badge/OpenCV-4.12+-green.svg)
![YOLO](https://img.shields.io/badge/YOLO-v8-orange.svg)
![CustomTkinter](https://img.shields.io/badge/CustomTkinter-5.2+-purple.svg)

## ✨ Features

- **25-minute work sessions** with 5-minute breaks
- **Real-time human detection** using YOLOv8
- **Modern dark theme UI** with CustomTkinter
- **Automatic timer pause/resume** based on presence
- **Audio alerts** when you leave your desk
- **Session history** with persistent storage
- **macOS camera permissions** handling

## 🛠️ Installation

### Prerequisites
- Python 3.13+
- Webcam
- Audio output capability

### Setup
```bash
git clone <your-repo-url>
cd visual_pomodoro
python3 -m venv pomodoro_env
source pomodoro_env/bin/activate
pip install -r requirements.txt
```

## 🚀 Usage

```bash
python3 pomodoro_app.py
```

1. Allow camera access when prompted
2. Click "Start Session" to begin
3. Stay at your desk - detection system monitors presence
4. Timer automatically pauses when you leave

## 📦 Dependencies

- `customtkinter` - Modern UI framework
- `ultralytics` - YOLO model implementation
- `opencv-python` - Computer vision
- `Pillow` - Image processing
- `numpy` - Numerical operations

## 📁 Project Structure

```
visual_pomodoro/
├── pomodoro_app.py           # Main application
├── requirements.txt           # Dependencies
├── README.md                  # This file
└── yolov8n.pt                # Detection model
```

## 🔧 Technical Details

- **Multi-threaded architecture** - Video processing separate from GUI
- **YOLOv8 nano model** - Real-time detection at 30 FPS
- **Thread-safe operations** - Safe GUI updates from background threads
- **JSON persistence** - Session history storage


## 📄 License

MIT License

---

**Built with Python, computer vision, and modern UI technologies.**
