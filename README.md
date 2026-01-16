# OpenCV Projects Collection

This repository contains a collection of computer vision projects implemented using OpenCV and Python. Each project is contained within a Jupyter Notebook and focuses on specific computer vision tasks ranging from basic face detection to social distancing monitoring.

## Projects Overview

### 1. Face Detection
- **File**: `face detection.ipynb`
- **Description**: This notebook demonstrates the fundamentals of face detection using Haar Cascade Classifiers. It covers:
  - Loading and displaying images.
  - Converting images to grayscale for processing.
  - Detecting faces and drawing bounding boxes around them.
  - Basic drawing operations (lines, circles) and adding text to images.
- **Key Dependencies**: `cv2`, `numpy`.
- **Required Assets**: `face.xml` (Haar Cascade), `myfirst.png` (Input image).

### 2. Video Playback & Live Face Monitoring
- **File**: `playing video.ipynb`
- **Description**: Explores video capture and processing capabilities. Key features include:
  - Capturing video from a live webcam feed (`cv2.VideoCapture(0)`).
  - Playing video from a file (`vt.mp4`).
  - Real-time face detection on video streams with visual indicators (rectangles and labels).
  - interactive controls to quit ('q') or save frames ('z').
- **Key Dependencies**: `cv2`.
- **Required Assets**: `face.xml`, `vt.mp4`.

### 3. Social Distancing - Full Body Detection
- **File**: `social distancing body.ipynb`
- **Description**: Focuses on detecting full-body figures in images. This can be used for crowd analysis or analyzing social distancing compliance in broader views.
- **Key Dependencies**: `cv2`, `numpy`.
- **Required Assets**: `haarcascade_fullbody.xml`, `TB.jpg`.

### 4. Social Distancing - Face Proximity Detection
- **File**: `social distancing faces.ipynb`
- **Description**: A specialized application for monitoring social distancing based on face proximity.
  - Detects multiple faces in a single image.
  - Calculates the Euclidean distance between the centroids of detected faces.
  - Visualizes violations by drawing red lines between faces that are closer than a set threshold (300 pixels) and flagging them in the console.
- **Key Dependencies**: `cv2`, `math` (standard library).
- **Required Assets**: `face.xml`, `i.jpg`.

## Getting Started

### Prerequisites

Ensure you have Python installed. It is recommended to use a virtual environment.

### Installation

1. Clone this repository.
2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

### Running the Projects

Launch Jupyter Notebook to view and run the projects:
```bash
jupyter notebook
```

## Note on Missing Assets

The scripts reference several external files that may not be present in the repository. To run the code successfully, you will need to provide the following:

- **Haar Cascade Models**:
  - `face.xml` (typically `haarcascade_frontalface_default.xml`)
  - `haarcascade_fullbody.xml`
  - *Download these from the [OpenCV GitHub repository](https://github.com/opencv/opencv/tree/master/data/haarcascades).*

- **Media Files**:
  - `myfirst.png`
  - `vt.mp4`
  - `TB.jpg`
  - `i.jpg`