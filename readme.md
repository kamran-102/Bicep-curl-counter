#  Bicep Curl Counter

### Overview

This repository contains a Python script that counts bicep curls in a video by analyzing the angle between the shoulder, elbow, and wrist. The video is processed frame-by-frame to detect and track the position of the joints. When the arm completes a full curl (from "down" to "up" stage), the counter is incremented.

### Dependencies

- **Python 3.x**
- **numpy**
- **mediapipe**
- **opencv-python**

### Installation

1. **Install Python 3.x:** Ensure that Python 3.x is installed on your system.
2. **Install Required Libraries:** Run the following command to install the necessary Python libraries:
    ```bash
    pip install numpy mediapipe opencv-python
    ```
3. **Clone the Repository:** Download or clone this repository to your local machine.

## Usage

1. **Set VideoPath**:
   - Modify the `File_path` variable to match the name of your video file.

2. **Run the Script**:
    ```bash
    python bicep_curl_counter.py
    ```

3. **Real-Time Bicep curl Counting**:
   - The video will be displayed in a window. The curl counter and stage information will be overlaid on the video.

4. Press 'q' to exit the video window and stop the program.

### Disclaimer

"This code is provided for educational and informational purposes only. The accuracy of the bicep curl counting relies heavily on the correct detection and tracking of body landmarks, which can be influenced by various factors such as camera angle, lighting, and the user's form. The angle thresholds (`130` for "down" and `100` for "up") are set based on general observations and may not be suitable for all users or exercises. You may need to adjust these thresholds depending on the specific video, the form of the exercise, or individual body mechanics."
