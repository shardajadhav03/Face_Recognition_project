# Face Recognition Project
## Introduction
This project implements a face recognition system using Python and OpenCV. The system can capture and store images of individuals from a webcam, encode the facial features, and recognize faces in real-time video streams. It is an ideal project for learning about computer vision, facial recognition, and integrating AI-powered features into applications.

## Features
1. Image Capture: Allows users to store images of their faces into uniquely named folders.
2. Face Encoding: Encodes facial features for efficient recognition.
3. Real-Time Recognition: Detects and identifies faces in live webcam video streams.
4. Scalability: Easily extendable to include more individuals and data.

## Requirements
Before running this project, ensure the following libraries and tools are installed:

- Python 3.11 or above
- OpenCV
- dlib
- Face Recognition
- cmake (used for dlib)

## Special Installation Note
While installing the face_recognition library, you might encounter an error. To resolve this:

- Download the precompiled dlib-19.24.1-cp311-cp311-win_amd64.whl file.
- Install it using the command: pip install dlib-19.24.1-cp311-cp311-win_amd64.whl.

## Project Structure
- Image Folder: Contains subfolders named after individuals, storing their captured face images.
- Face Encoding Functionality: Generates unique encodings for each face and associates them with the corresponding name.
- Real-Time Recognition: Utilizes webcam input to identify faces and displays results on a video feed.

## Workflow
1. Setup and Preparation:

    - Create folders for each individual in the image directory.
    - Capture multiple images using the webcam and store them in the respective folders.
      
2. Encoding Faces:

    - The project scans the image directory, processes each image, and generates face encodings.

3. Real-Time Detection:

    - A live video feed from the webcam is analyzed.
    - If a face matches a known encoding, the system displays the individual's name.
    - Unknown faces are labeled as "Unknown."

## Challenges and Solutions
1. Installation Errors:
    - Resolved by manually installing the necessary dlib library.
2. Image Processing Errors:
    - Non-image files (e.g., .ipynb_checkpoints) are skipped to ensure smooth processing.

## Usage
1. Clone this repository to your local machine.
2. Install the required libraries as outlined in the requirements.
3. Capture face images and store them in individual folders.
4. Run the face recognition system to detect and identify faces in real-time.
