# YOLOv3 Object Detection from Scratch

This repository contains an implementation of YOLOv3 (You Only Look Once version 3) object detection algorithm from scratch using PyTorch. YOLOv3 is a popular object detection algorithm that is fast and efficient, capable of detecting objects in real-time.

## Prerequisites

- Python 3.6 or later
- PyTorch
- NumPy
- OpenCV
- PIL
- albumentations
- pandas
- matplotlib
- tqdm

You can install the required packages using the following command:

```bash
pip install torch numpy opencv-python pillow albumentations pandas matplotlib tqdm
```

## Usage

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your_username/yolov3-objectdetection-scratch.git
   cd yolov3-objectdetection-scratch
   ```

2. **Prepare the Dataset**

   Make sure that your dataset is organized in the following structure:

   ```
   dataset
   ├── images
   │   ├── image1.jpg
   │   ├── image2.jpg
   │   └── ...
   └── labels
       ├── image1.txt
       ├── image2.txt
       └── ...
   ```

   Each text file in the `labels` directory should contain the object annotations for the corresponding image, with one object per line formatted as follows:

   ```
   class x_center y_center width height
   ```

   - `class`: The object class id (integer)
   - `x_center`, `y_center`: The center coordinates of the bounding box (relative to the width and height of the image)
   - `width`, `height`: The width and height of the bounding box (relative to the width and height of the image)

3. **Modify the Configuration**

   Update the configuration section in the script to match your dataset and training preferences:

   ```python
   # Configuration
   batch_size = 32
   learning_rate = 1e-5
   epochs = 20
   image_size = 416
   class_labels = ["class1", "class2", "class3", ...]
   ```

4. **Train the Model**

   Run the script to start the training process:

   ```bash
   python yolov3.py
   ```

5. **Visualize the Results**

   After training, you can use the `plot_image` function to visualize the object detection results on a sample image.

## Features

- YOLOv3 object detection algorithm implemented in PyTorch
- Custom dataset loading and preprocessing
- Data augmentation using albumentations
- Intersection over Union (IoU) and Non-Maximum Suppression (NMS) for accurate bounding box predictions
- Model checkpoint saving and loading
- Real-time object detection visualization

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check [issues page](https://github.com/your_username/yolov3-objectdetection-scratch/issues).
