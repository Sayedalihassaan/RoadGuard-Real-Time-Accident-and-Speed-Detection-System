
# RoadGuard Real-Time Accident and Speed Detection System 🚗💥🏎️

![RoadGuard Banner]![image](https://github.com/user-attachments/assets/08e64108-d3f5-4468-870e-1d79a176bc57)
) <!-- You can add a banner image or screenshot of the project -->

## Overview
The **RoadGuard Real-Time Accident and Speed Detection System** is a computer vision-based system designed to monitor vehicular traffic and detect accidents in real-time. By utilizing **YOLOv8** object detection and **OpenCV**, this system can:
- Detect vehicles in a video stream.
- Estimate their speeds.
- Detect sudden speed drops, indicating potential accidents.
- Provide real-time alerts to improve road safety.

## Key Features 🚀
- **Accurate Vehicle Detection**: Uses state-of-the-art YOLOv8 for precise vehicle localization.
- **Speed Estimation**: Calculates real-time vehicle speeds based on pixel-to-meter conversion.
- **Accident Detection**: Identifies potential collisions by tracking abnormal speed drops.
- **Real-time Visualization**: Displays detected vehicles, speed, and alerts on the video stream.
- **Customizable Parameters**: Easily adjust speed thresholds, frame rates, and distance conversion for different scenarios.

## How It Works 🛠️
1. **Object Detection**: YOLOv8 is used to detect vehicles from the input video.
2. **Speed Calculation**: The Euclidean distance between vehicle centers is computed to estimate speed.
3. **Accident Detection**: If a significant drop in speed is detected, an alert is generated to indicate a potential accident.

## Project Structure 📂
```bash
.
├── tracker.py             # Tracking logic for vehicle movement
├── coco1.txt              # COCO class labels for vehicle detection
├── best (1).pt            # Pre-trained YOLOv8 model
├── cr.mp4                 # Sample video file (replace with your own)
├── main.py                # Main script for accident and speed detection
└── README.md              # Project documentation
```

## Installation 🔧
1. **Clone the Repository**
    ```bash
    git clone https://github.com/Sayedalihassaan/RoadGuard-Accident-Speed-Detection.git
    ```
2. **Install Dependencies**
    Make sure you have Python and pip installed. Then install the necessary libraries:
    ```bash
    pip install opencv-python cvzone ultralytics numpy
    ```
3. **Download YOLOv8 Model**
    Download the pre-trained YOLOv8 model and place it in the project directory.

4. **Run the System**
    ```bash
    python main.py
    ```

## Usage 🎯
- You can test the system using the provided `cr.mp4` video, or replace it with your own video by modifying the path in `main.py`.

## Example Output 📊
![Example Output](https://your_output_screenshot_here) <!-- Add a screenshot of the output -->

- Detected vehicles with real-time speed estimates displayed on the frame.
- **Accident Alerts** in red, triggered when a sudden speed drop is detected.

## Customization ✨
- Adjust the `distance_conversion_factor` in `main.py` for different pixel-to-meter conversions.
- Modify the speed threshold or detection parameters for different vehicle types.

## Future Enhancements 🔮
- [ ] Add functionality to log accidents in a database.
- [ ] Integrate with external APIs for real-time road safety monitoring.
- [ ] Extend the system to handle pedestrian and cyclist detection.

## Contribution 🤝
Contributions are welcome! If you have suggestions or improvements, feel free to fork the repository and submit a pull request.

## License 📄
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

