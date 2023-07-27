# RealTime-FaceRecognition

## Description:
This Python script performs face recognition in real-time using the `face_recognition` library and OpenCV. It can recognize faces from a live video stream and display the names of known individuals along with their confidence levels based on facial similarity. The script uses pre-registered face images from the `faces` folder to build a database of known faces.

The face recognition algorithm calculates the Euclidean distance between the features of detected faces and known faces to determine the level of similarity. A confidence score is assigned to each recognized face, indicating the percentage of similarity. The confidence score is also written to a `results.txt` file for future reference.

## Requirements:

- Python 3.x
- OpenCV (`cv2`)
- face_recognition library (`face_recognition`)

## Setup:

1. Make sure you have Python 3.x installed on your system.
2. Install the required libraries using `pip`:
   ```
   pip install opencv-python face-recognition
   ```
3. Place the images of known faces in the `faces` folder.

## Usage:

1. Execute the script by running the following command in the terminal or command prompt:
   ```
   python face_recognition_script.py
   ```
2. The script will access your default camera and start recognizing faces in the live video stream.
3. Recognized faces will be annotated with bounding boxes and labeled with names and confidence levels.
4. Press the 'esc' key to exit the application.
