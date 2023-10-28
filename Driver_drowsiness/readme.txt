# Driver Drowsiness Detection System

## Introduction
The Driver Drowsiness Detection System is an innovative solution aimed at enhancing road safety by monitoring the driver's state and providing real-time alerts in case of drowsiness or sleep. Leveraging advanced computer vision techniques and deep learning-based facial landmark detection, this system achieves a significant accuracy of 81.6%.

## System Architecture
This system employs a Raspberry Pi (Version 3 Model B+) as its core computing unit, coupled with a Camera Module V2 for capturing real-time video feed. The Raspberry Pi 3 Model B+ is equipped with a 1.4GHz 64-bit quad-core processor, dual-band wireless LAN, and full-size GPIO headers, making it an ideal choice for this project. The Camera Module V2 features an 8-megapixel Sony IMX219 sensor and supports 1080p30, 720p60, and VGA90 video modes, providing clear and high-resolution images crucial for accurate facial landmark detection.

## Pre-requisites
- Raspberry Pi 3 Model B+
- Camera Module V2
- MicroSD card (minimum 8GB)
- Raspberry Pi power supply
- Keyboard, mouse, and monitor for initial setup

## Installation and Setup
1. Download the Raspbian operating system image and flash it onto the MicroSD card.
2. Insert the MicroSD card into the Raspberry Pi and connect all necessary peripherals.
3. Power up the Raspberry Pi and complete the initial setup.
4. Open a terminal and run `sudo raspi-config` to enable the camera interface.
5. Reboot the Raspberry Pi to apply the changes.
6. Install the necessary dependencies by running:
    ```bash
    sudo apt-get update
    sudo apt-get install python3 python3-pip python3-numpy
    pip3 install opencv-python dlib imutils
    ```
7. Clone the project repository to your Raspberry Pi.
    ```bash
    git clone <repository-url>
    cd <repository-directory>
    ```

## Deployment
1. Connect the Camera Module V2 to the Raspberry Pi using the CSI port.
2. Navigate to the project directory.
3. Run the main script to start the driver drowsiness detection system.
    ```bash
    python3 main.py
    ```
4. The system will now analyze the driver's state and display the result in real-time. The possible states are "Active :)", "Drowsy!", and "SLEEPING!!!".

## Image Examples
The repository includes example images demonstrating the different states of the driver:
- `active.png`: Shows the driver in an active state.
- `drowsy.png`: Shows the driver in a drowsy state.
- `sleep.png`: Shows the driver in a sleeping state.

## Technical Details
The system utilizes a machine learning model with facial landmark detection to monitor the driver's eye blink rate. Based on the blink rate and duration, the system categorizes the driver's state into active, drowsy, or sleeping. The deep learning model and computer vision techniques ensure accurate and reliable monitoring, resulting in a significant accuracy of 81.6%.

## Conclusion
The Driver Drowsiness Detection System is a pivotal step towards enhancing road safety and preventing accidents caused by drowsy driving. With its high accuracy and real-time monitoring capabilities, it serves as a reliable assistant for drivers, ensuring they remain alert and safe on the road.

## License
This project is open-source and available under the MIT License.
