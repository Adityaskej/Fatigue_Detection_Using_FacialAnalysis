# Fatigue_Detection_Using_FacialAnalysis
Fatigue_Detection_Using_Facial_Analysis PROJECT
Project Overview
This project implements a real-time fatigue detection system using facial landmark analysis. It captures video from the webcam and monitors key indicators of drowsiness, including:

Continuous eye closure
Frequent yawning
Abnormal head tilt

The system utilizes MediaPipe and OpenCV for facial landmark detection and video processing.

Technologies Used
Python – Core programming language
OpenCV – Real-time video capture and visualization
MediaPipe – Facial mesh and landmark detection
NumPy – Geometric and mathematical calculations
VS Code – Code development and execution environment

Files Included

fatigue_detector_combined.py – Main script integrating all detection features
eye_closure_detection.py – Detects continuous eye closure using EAR (Eye Aspect Ratio)
yawn_detection.py – Detects yawning based on lip distance
head_tilt_detection.py – Identifies abnormal head tilt using face geometry
face_mesh_test.py – Test script for MediaPipe face mesh functionality
requirements.txt – Lists all required Python packages

System Features
1. Eye Closure Detection
Calculates Eye Aspect Ratio (EAR)
Triggers an alert if eyes remain closed for ≥ 2 seconds

2. Yawn Detection

Measures vertical lip distance
Monitors yawns within a 60-second window
Triggers an alert if 3 or more yawns are detected

3. Head Tilt Detection

Computes the tilt angle between eyes
Triggers an alert if the tilt exceeds ±15°

System Workflow

Accesses webcam stream

Detects facial landmarks using MediaPipe

Calculates EAR, lip distance, and head tilt angle

Compares measurements with set thresholds:
EAR < 0.25 for ≥ 2 seconds
3+ yawns in 60 seconds
Head tilt angle > ±15°
Displays visual alerts on screen when thresholds are exceeded

Future Improvements
Add audio alerts for enhanced visibility
Implement logging of alert timestamps for performance analysis and reporting

Contact
Aditya Sasikumar
📧 Email: adityasasikumar422@gmail.com
