# Car and Truck Object Tracking Using YOLOv8

This project demonstrates real-time object tracking of cars and trucks in video streams using the YOLOv8 model from Ultralytics, integrated with OpenCV for video processing and PyTorch for model inference. The solution detects and tracks moving vehicles, providing bounding boxes and real-time tracking in a video feed.

## Features
- **Object Detection and Tracking**: Detects and tracks cars and trucks in a video using YOLOv8.
- **Real-time Processing**: Efficient and fast processing of video streams with accurate object detection.
- **YOLOv8**: Utilizes Ultralytics' pre-trained YOLOv8 model for high-performance object detection.
- **Fine-Tuning**: The model has been fine-tuned on a custom dataset from Roboflow for improved accuracy in detecting cars and trucks.

## Project Overview

This project involves:
- Loading a pre-trained YOLOv8 model, fine-tuned on a vehicle detection dataset for 50 epochs.
- Processing a video file and applying the object detection model to track cars and trucks.
- Using OpenCV to capture frames, run inference, and display bounding boxes on detected vehicles.

## Inference Pipeline

The core of this project is the `inference` function, which takes in a video file path, applies the YOLOv8 model to detect cars and trucks, and outputs the processed video with tracking.

### Example:

```python
# Path to input video and path to save output video
input_video_path = "path/to/video.mp4"
output_video_path = "path/to/output_video.mp4"

# Run the object tracking inference
network_inference(input_video_path, output_video_path)
```

## Requirements

- Python 3.x
- Ultralytics YOLOv8
- OpenCV
- PyTorch


## Files

- `TrackingVehicle.ipynb`: Contains the `network_inference` function for performing object detection and tracking.
- `README.md`: Project documentation.

## Pre-trained Model

You can download the fine-tuned model weights:

[YOLOv8 Model Weights](https://drive.google.com/file/d/1fjaLUcFvMKgVKRzlqL1fVKExo5Dnirs-/view?usp=sharing)

## Demo

### Input Video:
[Input Video Link](https://drive.google.com/file/d/1fjaLUcFvMKgVKRzlqL1fVKExo5Dnirs-/view?usp=sharing)

### Output Video:
[Output Video Link](https://drive.google.com/file/d/1S8vI-5KaY_IAg6ytGkSWy3cvExvJZtNt/view?usp=sharing)

## Results

- Cars and trucks are detected and tracked in the video.
- Bounding boxes show real-time tracking of the vehicles.
- The YOLOv8 model was fine-tuned on a dataset from Roboflow, leading to enhanced detection accuracy.

## Future Enhancements

- Improve tracking algorithm for better performance on occluded objects.
- Integrate with more complex tracking methods.
