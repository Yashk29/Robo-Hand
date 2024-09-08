# Robotic Hand with Gesture Recognition

This project involves creating a robotic hand using Arduino and OpenCV with gesture recognition. The hand is controlled based on gestures detected through the camera, and the prototype is developed using cardboard. The project also integrates with a web-based interface using Flask for interaction with the hardware.

## Features

- Gesture Recognition: Uses OpenCV to detect hand gestures and control the robotic hand accordingly.
- Arduino Integration: Controls the motors and movements of the robotic hand.
- Flask Backend: Provides a web interface for real-time control and interaction with the robotic hand.
- Cross-Origin Resource Sharing (CORS): Enables communication between the frontend and backend securely.
- Serial Communication: Utilizes serial communication to send commands to the Arduino.

## Libraries and Tools Used

- [cvzone](https://github.com/cvzone/cvzone): A library that simplifies computer vision tasks like gesture recognition and hand tracking.
- [numpy](https://numpy.org/): A fundamental package for scientific computing in Python.
- [myserial](https://pypi.org/project/pySerial/): A Python library to establish serial communication between the Arduino and the computer.
- [opencv-python](https://pypi.org/project/opencv-python/): OpenCV library for computer vision tasks such as gesture recognition.
- [flask](https://flask.palletsprojects.com/): A micro web framework written in Python used for creating the web interface.
- [flask-cors](https://pypi.org/project/Flask-Cors/): Handles Cross-Origin Resource Sharing (CORS) to allow cross-origin AJAX requests to the Flask server.

## Installation

To install the required libraries, run the following command:

```bash
pip install cvzone numpy myserial opencv-python flask flask-cors
```

## How to Run the Project

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo.git
   ```

2. Navigate to the project directory:

   ```bash
   cd your-repo
   ```

3. Install the required libraries:

   ```bash
   pip install -r requirements.txt
   ```

4. Connect the Arduino to your computer.

5. Run the Flask server:

   ```bash
   python app.py
   ```

6. Open your browser and go to `http://127.0.0.1:5000` to access the web interface.

## How It Works

- The cvzone and OpenCV libraries are used to track hand gestures via a camera.
- The recognized gestures are sent via serial communication (myserial) to the Arduino, which controls the motors of the robotic hand.
- The Flask web interface allows users to interact with the robotic hand in real-time.

## Future Enhancements

- Improving the accuracy of gesture recognition.
- Adding more gesture-based functionalities.
- Upgrading the robotic hand from cardboard to a more durable material.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## My Role as Teammate

- Gesture Recognition Array: I created a system to detect finger movements, using an array to represent the state of each finger (up as 1, down as 0). This is a crucial part of translating gestures into 
  commands for the robotic hand.
- Frontend Development: I built the user interface, allowing users to operate the robotic hand through a web-based control panel.

