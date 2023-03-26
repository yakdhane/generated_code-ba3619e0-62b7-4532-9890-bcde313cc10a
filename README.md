# Facial Recognition App

This is a facial recognition app built with Python. It uses the `face_recognition` library to recognize faces in real-time using a webcam. The app can be trained to recognize multiple faces and can be used for various applications.

## Dependencies

The app requires the following dependencies:

- Python 3.6 or higher
- OpenCV
- face_recognition
- numpy

## Installation

1. Clone the repository
2. Install the dependencies using `pip install -r requirements.txt`

## Usage

1. Add images of the people you want to recognize in the `images` folder. The images should be named after the person's name, e.g., `person1.jpg`, `person2.jpg`, etc.
2. Run the `main.py` file using `python main.py`
3. The app will start the webcam and recognize faces in real-time.

## Docker

A Dockerfile is included in the repository. To run the app using Docker, follow these steps:

1. Install Docker on your machine
2. Build the Docker image using `docker build -t facial-recognition-app .`
3. Run the Docker container using `docker run -p 80:80 facial-recognition-app`

## Files

- `face_detection.py`: Contains the code for detecting faces in an image using OpenCV.
- `face_encoding.py`: Contains the code for encoding a face image using the `face_recognition` library.
- `main.py`: The main file that runs the facial recognition app.
- `encodings.pickle`: A pickle file that contains the face encodings of the people to be recognized.
- `haarcascade_frontalface_default.xml`: A pre-trained classifier for detecting faces in an image.
- `images/`: A folder that contains the images of the people to be recognized.
- `Dockerfile`: A file that contains the instructions for building a Docker image of the app.