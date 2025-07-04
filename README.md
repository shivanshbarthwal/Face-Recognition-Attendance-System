# 🧑‍💼 Face Recognition Attendance System

A real-time face recognition attendance system using Python, OpenCV, and the `face_recognition` library. This application detects known faces through your webcam and marks attendance by logging names and timestamps into a CSV file.

---

## 📸 Features

- Real-time face detection from webcam
- Recognizes multiple known faces
- Logs attendance with name and time
- Saves daily attendance in a CSV file named by date

---

## 🛠️ Technology Stack

- **Python 3**
- **face_recognition** – for face detection and encoding
- **OpenCV** – for video processing and display
- **NumPy** – for array operations
- **CSV & datetime** – for logging attendance

---

## 📦 Installation

Install the required Python libraries:

```bash
pip install opencv-python face_recognition numpy
```

> Note: `face_recognition` requires `dlib`. You may need CMake and Visual Studio Build Tools on Windows.

---

## 🚀 How to Run

1. Place all face images in a folder named `faces/`  
   Example:
   ```
   faces/shivansh.jpg
   faces/aman.jpg
   faces/nisha.jpg
   faces/rahul.jpg
   ```

2. Run the script:

```bash
python attendance.py
```

3. Press `q` to quit the webcam and save attendance.

---

## 📁 File Structure

```
face-attendance/
├── attendance.py           # Main Python script
├── faces/                  # Folder containing reference images
│   ├── shivansh.jpg
│   ├── aman.jpg
│   ├── nisha.jpg
│   └── rahul.jpg
├── 04-07-2025.csv          # Sample output CSV (date-named)
├── README.md               # Documentation
```

---

## ✅ Output

A CSV file like `04-07-2025.csv` will be generated:

| Name     | Time     |
|----------|----------|
| Shivansh | 10:12:05 |
| Aman     | 10:13:44 |

---

## 🛡️ Notes

- Ensure your camera has proper lighting for best recognition.
- File names and known face names must match accordingly.
- Works best with high-quality, front-facing images.
