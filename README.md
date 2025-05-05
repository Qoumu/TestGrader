# TestGrader

This project implements a low-cost, efficient automated test grading system using ESP32-CAM for image capture, ESP8266 for control signaling, and MQTT protocol for wireless communication with a central laptop for processing and result management.

### System Components

ESP32-CAM: Acts as the camera module, responsible for capturing images of test papers (either MCQ sheets or OMR-like forms).

ESP8266 NodeMCU: Works as the controller unit, signaling when a new test is ready for capture and possibly driving mechanical parts (e.g., paper feed, motor).

Laptop (PC): Serves as the processing unit, running an image processing script (e.g., Python + OpenCV) to analyze the captured images and extract the test results.

MQTT Broker (e.g., Mosquitto): Acts as the communication hub, enabling real-time message exchange between ESP modules and the laptop.
