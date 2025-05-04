# Facial Emotion Detector

An Android application that detects and displays facial emotions in real-time using MediaPipe and OpenCV.

## Features

- Real-time facial emotion detection
- Front camera integration with CameraX
- Supports detection of 5 emotions: Happy, Sad, Angry, Surprised, and Neutral
- Uses MediaPipe Face Landmarker for facial feature detection
- Processes emotions using both blend shapes and geometric feature analysis

## Technologies Used

- Android SDK
- CameraX
- MediaPipe Tasks Vision Library
- OpenCV for Android
- Java

## Requirements

- Android Studio Chipmunk (2022.1) or newer
- Android SDK 24 or higher
- Android device with a front-facing camera

## Setup and Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/FacialEmotionDetector.git
   ```

2. Open the project in Android Studio

3. Build and run the application on your Android device

## How It Works

The application uses the following components:

1. **CameraHelper**: Utilities for camera image conversion and manipulation
2. **FaceMeshProcessor**: Processes camera frames using MediaPipe to detect facial landmarks
3. **EmotionDetector**: Analyzes facial landmarks to detect emotions
4. **MainActivity**: Main UI and camera setup

The emotion detection works in two ways:
- Using MediaPipe's face blendshapes when available
- Using geometric analysis of facial landmarks when blendshapes aren't available

## Permissions

The application requires the following permissions:
- Camera access

## License

[Add your license information here]

## Acknowledgments

- MediaPipe by Google
- OpenCV contributors
