# Drishti: Smart Traffic Management System

### Project Overview
Developed an adaptive traffic control system that leverages computer vision to dynamically manage traffic signals based on actual road demand. The system optimizes traffic flow by prioritizing high-congestion lanes and emergency vehicles, improving queue clearance while ensuring fairness to all lanes.

### Key Features
* **Adaptive Signal Control:** Dynamically adjusts traffic signals based on real-time congestion scores.
* **Emergency Vehicle Prioritization:** Specialized logic to detect and prioritize emergency vehicles to ensure rapid transit.
* **Lane Starvation Prevention:** Integrated fairness algorithms to ensure no lane is left waiting indefinitely regardless of demand.
* **Real-time Monitoring:** Uses high-speed object detection to assess road demand and clear queues efficiently.

### Tech Stack
* **Computer Vision:** YOLOv8, OpenCV, and ONNX Format.
* **Hardware:** Raspberry Pi 5, 3x Cameras, GPIO Control, and LED Traffic Signal Modules.
* **Programming:** Python.

### How it Works
1. **Detection:** Cameras capture live feeds of multiple lanes.
2. **Analysis:** YOLOv8 models process the frames to count vehicles and identify emergency units.
3. **Control:** The system calculates a congestion score and triggers GPIO pins on the Raspberry Pi to operate the LED traffic modules.
