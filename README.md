# Driver-Drowsiness-Detection-System

## Overview

This project is a Driver Drowsiness Detection System developed using Python, OpenCV, and MediaPipe. The main purpose of this project is to detect signs of driver fatigue by monitoring the driver's eye movements through a webcam.

When the system detects that the driver's eyes remain closed for a certain period of time, it displays a warning message and triggers an alarm sound to alert the driver.

This project was developed as a learning project to understand computer vision concepts and real-time facial landmark detection.

---

## Features

* Real-time face and eye detection using webcam
* Eye Aspect Ratio (EAR) calculation
* Detects prolonged eye closure
* Displays drowsiness warning on screen
* Plays alarm sound when drowsiness is detected
* Simple and user-friendly implementation
* No external APIs are used

---

## Technologies Used

* Python
* OpenCV
* MediaPipe
* NumPy
* Playsound

---

## Project Structure

Driver-Drowsiness-Detection/

├── main.py

├── alarm.wav

├── requirements.txt

└── README.md

---

## Installation

1. Clone the repository:

git clone <your-github-repository-link>

2. Move into the project folder:

cd Driver-Drowsiness-Detection

3. Install the required libraries:

pip install -r requirements.txt

---

## Running the Project

Follow the steps below to run the Driver Drowsiness Detection System on your computer.

### Step 1: Open the Project Folder

Open VS Code and navigate to the project folder:

```bash
cd Driver-Drowsiness-Detection
```

### Step 2: Install Required Dependencies

Install all required Python libraries using:

```bash
pip install -r requirements.txt
```

If any dependency is missing, install them manually:

```bash
pip install mediapipe==0.10.14
pip install opencv-python
pip install numpy
pip install playsound==1.2.2
```

### Step 3: Run the Application

Execute the following command in the terminal:

```bash
python main.py
```

### Step 4: Start Monitoring

After running the program:

* The webcam will open automatically.
* The system will detect the driver's face and eyes in real time.
* Eye movements will be continuously monitored using facial landmarks.
* The current status will be displayed on the screen.

### Drowsiness Detection

If the driver's eyes remain closed for a few seconds:

* A warning message saying **"DROWSINESS ALERT!"** will appear on the screen.
* An alarm sound will be played to alert the driver.
* The system will continue monitoring until the driver's eyes reopen.

### Exit the Application

To close the application:

* Press the **ESC** key on the keyboard, or
* Click the close button on the webcam window.

The webcam will stop and the program will terminate safely.

After running the program, the webcam will start automatically.

The system will continuously monitor the driver's eyes. If the eyes remain closed for a few seconds, a warning message will be displayed and an alarm sound will be played.

---

## How It Works

The system uses MediaPipe Face Mesh to detect facial landmarks around the eyes.

The Eye Aspect Ratio (EAR) is calculated using selected eye landmark points. When the EAR value falls below a predefined threshold for multiple consecutive frames, the system considers the driver to be drowsy.

Once drowsiness is detected:

* A warning message appears on the screen.
* An alarm sound is triggered.
* The driver is alerted to stay attentive.

---

## Challenges Faced

During development, one of the main challenges was setting up facial landmark detection libraries and ensuring compatibility with the Python version being used. Another challenge was selecting appropriate threshold values so that normal blinking would not trigger false alerts.

---

## Future Improvements

* Yawning detection
* Head pose estimation
* Mobile application integration
* Performance optimization for low-end devices
* Driver monitoring dashboard

---

## Conclusion

This project helped me understand the basics of computer vision, facial landmark detection, and real-time video processing. It demonstrates how technology can be used to improve road safety by helping detect driver fatigue before it leads to accidents.

---

## Author

Paruchuri Venkatesh
=======
# Driver-Drowsiness-Detection
>>>>>>> 623d16ceb874a955522f069d994e89470fba63c0
