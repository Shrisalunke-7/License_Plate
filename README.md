# License Plate Recognition

License plate recognition is a significant challenge in computer vision, involving two key tasks:

1. **License Plate Detection**: Identifying and locating license plates in vehicle images.
2. **Character Recognition**: Recognizing and extracting the alphanumeric text from the detected license plates.

This project leverages a dataset comprising vehicle and license plate images, organized into distinct training and test sets, to achieve these goals.

## Dataset Description

The dataset is divided into three distinct sets, each designed to support specific aspects of the task:

### 1. Training Set 1
- **Images**: 900 images of vehicles, each containing a single car and its corresponding license plate.
- **Annotations**: Coordinates of bounding boxes that outline the license plates in the images. The format for each bounding box is:
  - `ymin, xmin, ymax, xmax`

### 2. Training Set 2
- **Images**: 900 images focusing solely on license plates.
- **Annotations**: Alphanumeric characters present on each license plate.

### 3. Test Set
- **Images**: 201 images, structured similarly to Training Set 1, featuring vehicles and their license plates.
- **Task**: 
  - Detect and locate license plates in the images.
  - Recognize and extract the alphanumeric text from the detected license plates.

## Objectives

The primary objectives of this project are:

1. **License Plate Detection**: Train a model to identify and locate the license plates affixed to vehicles in images.
2. **Character Recognition**: Train a model to perform optical character recognition (OCR) on license plates and extract the alphanumeric text.

## Evaluation Criteria

The model's performance during the evaluation phase will be assessed based solely on the accuracy of **character recognition**. This requires precise detection and OCR capabilities to ensure high accuracy in recognizing the alphanumeric text on license plates.

## Key Challenges

- Detecting license plates under varying conditions (e.g., lighting, angles, and occlusions).
- Accurately recognizing characters, considering variations in font styles, sizes, and image quality.

## Usage Instructions

To utilize this dataset effectively, follow these steps:

1. Train a detection model using **Training Set 1** to identify license plates in images.
2. Train a recognition model using **Training Set 2** to decode the alphanumeric text on license plates.
3. Evaluate the combined system on the **Test Set** to measure its performance in detecting license plates and recognizing the characters accurately.

By tackling this challenge, we aim to build a robust system for automated license plate recognition that can be deployed in real-world applications.
