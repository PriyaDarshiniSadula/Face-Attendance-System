# Face Attendance System

This is a simple project I worked on to automate attendance using face recognition.  
It uses OpenCV and the `face_recognition` library to detect and recognize faces from a webcam feed.

## How it works
- Add new faces to the dataset using `insert.py`.
- Train the system with `train.py`.
- Use `facerecog.py` to recognize faces and mark attendance in `attendance.csv`.
- `facedetec.py` can be used just for detecting faces without attendance.

## Setup
1. Create a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS / Linux
   venv\Scripts\activate      # Windows
   ```

2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
You can run scripts directly, for example:
```bash
python train.py
python facerecog.py
```

Or use the helper file for convenience:
```bash
python main.py train
python main.py recognize
```

## Notes
- Make sure the `tp/` folder contains images of the people you want to recognize.
- The recognized names will be saved into `attendance.csv`.
