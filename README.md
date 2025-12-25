# Pet Activity Monitoring using YOLOv8

A **real-time computer vision system** that detects pets (cats and dogs) through a live camera feed and analyzes their behavior using deep learning. The system classifies pet activities such as **playing, eating, and idle states** based on movement and object detection. It records annotated video output and logs activity changes with timestamps into a structured CSV file for further analysis.

Built using **YOLOv8, OpenCV, and Python**, this project demonstrates practical applications of AI in smart monitoring systems.

---

## 🔹 Features

- Real-time **pet detection** using YOLOv8
- Activity classification:
  - Playing
  - Eating
  - Sleeping / Idle
- Annotated **video recording** of pet activity
- **Activity logging** with timestamps into CSV
- Supports live webcam or video file input
- Lightweight and easy to run on a standard PC

---

## 🔹 Technologies Used

- **Python 3.11+**
- **YOLOv8 (Ultralytics)**
- **OpenCV** for video processing and annotation
- **Pandas** for activity log management
- **Datetime** for timestamping events

---

## 🔹 Installation
Install dependencies:

bash
Copy code
pip install -r requirements.txt
Note: Make sure to install NumPy 1.26.x to avoid compatibility issues with OpenCV and YOLOv8.

##  Usage
Make sure your webcam is connected (or replace with a video path in the code).

Run the main script:

bash
Copy code
python pet_activity_monitor.py
The system will:

Detect pets in real-time

Annotate frames with bounding boxes and activity labels

Record video to a timestamped .mp4 file

Log activity changes to pet_activity_log.csv

Press q to stop recording.

## Output

Video: pet_activity_recorded_YYYYMMDD_HHMMSS.mp4

Activity Log: pet_activity_log.csv with columns:

time → timestamp of activity change

activity → detected activity (Playing, Eating, Sleeping / Idle)

Example CSV:

time	activity
2025-12-25 16:30:12	Playing
2025-12-25 16:31:05	Eating
2025-12-25 16:32:40	Sleeping / Idle

## Future Improvements
Add multi-pet tracking

Detect specific toys or interactions

Integrate notifications when activity changes

Use more advanced behavior classification using pose estimation

Optimize for low-light environments

## References
YOLOv8 Documentation – Ultralytics

OpenCV Python Documentation

Pandas Documentation


