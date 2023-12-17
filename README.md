# Face Recognition System

## Description

#### This project implements a face recognition system with motion detection, email notifications, and video recording capabilities.  
The system captures video frames, detects motion, recognizes faces, and sends email notifications when unknown faces are detected. It also saves video clips of detected faces.

## Getting Started

### Clone the repository

```bash
git clone https://github.com/shlomoshtraus/finalProject.git
```

### go into the project directory

```bash
cd finalProject
```

### Install Required Libraries

```bash
pip install opencv-python face-recognition pillow
```

### create a folder data and inside it known_faces and videos folder's

```bash
mkdir data && cd data && mkdir known_faces videos && cd..
```

## Usage

Run `main.py` to start the face recognition system.  
The system will use the camera specified by the camera_index parameter (default is 0). a window will open showing the camera feed.  
Press 'q' to exit the system.

## configuration

In the file `face_recognizer.py` you can change the following parameters:

 * EMAIL: Your Gmail email address.
 * PASSWORD: Your Gmail password.
 * RECEIVER: Email address to receive notifications.
 * IMAGE_DIRECTORY: Directory containing images of known faces.
 * TOLERANCE: Face recognition tolerance level.
 * RANDOM_FRAMES_TO_SEND: Number of random frames to include in email notifications.
 * RECORDING_DURATION_THRESHOLD: Threshold for recording duration before saving video clip.

