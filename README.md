**Face Recognition Attendance System**
This project is a face recognition-based attendance system that detects faces from a live webcam feed and marks attendance in a CSV file. The system uses OpenCV for image processing and the face_recognition library for face detection and encoding.

**Requirements**
Python 3.x
OpenCV
face_recognition
numpy
pickle

1. Clone the repository :- git clone https://github.com/yourusername/face-recognition-attendance.git
2.Navigate to the project directory :- cd face-recognition-attendance
3.Install the required packages:- pip install -r requirements.txt


**Directory Structure**

face-recognition-attendance/
│
├── Student_image/
│   ├── student1.jpg
│   ├── student2.jpg
│   └── ...
│
├── Attendance.csv
│
├── attendance.py
│
└── README.md


`Student_image/ directory contains images of students with their names as the filenames (e.g., john_doe.jpg).
Attendance.csv file stores the attendance records.
attendance.py contains the main script for running the attendance system.
README.md is this file, providing information about the project.`

**Usage**
1.Place images of students in the Student_image directory. The filename should be the student's name (e.g., john_doe.jpg).
2.Run the script:python attendance.py
3.The webcam feed will open, and the system will start detecting faces. When a known face is detected, it will mark the attendance in Attendance.csv.

**Notes**
Ensure that the image filenames in the Student_image directory are unique and correspond to the names of the students.
The system scales down the webcam feed by 25% for faster processing. Adjust the scaling factor if needed.
The script currently only works with a single face per image. Ensure each student image has only one face.
**Contributing**
If you have any suggestions or improvements, feel free to create a pull request or open an issue.
