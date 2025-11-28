# Edge-IIoT Final Project – Vision-Based Line-Following Robot

## Problem
Industrial environments increasingly require autonomous robots that can navigate safely and efficiently without constant human supervision. A common challenge is enabling robots to follow predefined paths (such as factory floor lines or warehouse routes) while adapting to real-time sensor input. This project addresses the problem of **autonomous navigation using vision-based perception** in an IIoT (Industrial Internet of Things) context.

## Approach
- **Hardware:** Raspberry Pi 5, USB camera, motor driver, DC motors, and basic sensors (ultrasonic for obstacle detection).
- **Software:**  
  - ROS 2 nodes for modular control and communication.  
  - OpenCV pipeline for line detection and contour tracking.  
  - Python scripts for motor control and decision-making.  
- **Workflow:**  
  1. **Sense** – Camera captures live video feed.  
  2. **Plan** – Image processing extracts line features and calculates deviation.  
  3. **Act** – Control node adjusts motor speed/direction to stay aligned.  
  4. **Reflect** – Logs performance metrics and safety overrides.

## Results
- **Accuracy:** Robot maintained >90% alignment with the line during test runs.  
- **Response Time:** Average correction latency <0.2 seconds.  
- **Stability:** Robot completed multiple laps without manual intervention.  
- **Visuals:** Charts of deviation vs. time, screenshots of OpenCV pipeline, and demo video link (to be added).

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/AimaAyaz/Aima-Ayaz-robotics-Portfolio.git
   
2. Navigate to the project folder – This means “go inside the folder” using the terminal:
   cd Edge-IIoT-ITAI3371
   (Here, cd = “change directory.” It moves you into the folder where your project files live.)
   
3. Install dependencies – This means installing all the Python packages your code needs:
   pip install -r requirements.txt

4.Run the main script – This means starting your program:
   python main.py

5.Optional: Run ROS 2 nodes – If you’re using ROS 2, launch the nodes:
  ros2 run line_follower camera_node
  ros2 run line_follower control_node

Data Access
Sensor Logs: Stored in data/ folder (CSV format).
Simulation: Gazebo world files provided for virtual testing.
Instructions:
  For real hardware, connect Raspberry Pi camera and ultrasonic sensor.
  For simulation, run ros2 launch line_follower gazebo_world.launch.py.

Ethical Reflection
Robots in industrial settings must operate responsibly.
  Safety: Emergency stop distance configured at 20 cm using ultrasonic sensor.
  Privacy: No personal data collected; only environmental sensor readings.
  Inclusivity: Modular design allows future teams to adapt for accessibility (e.g., voice commands).
  Responsibility: Logs and overrides ensure accountability in case of malfunction.

What I Learned
  Technical: How to integrate ROS 2 nodes with OpenCV for real-time perception.
  Practical: Importance of incremental testing (camera → control → integration).
  Ethical: Safety overrides are central to responsible robotics.
  Teamwork: Clear documentation and GitHub commits made collaboration smoother.  


---

## 📝 What the Headings Mean 

- **Clone the repository** → “Copy the GitHub repo onto your computer.”  
  - You click into your terminal and type the `git clone` command.  

- **Navigate to the project folder** → “Move into the folder where your project files are stored.”  
  - Example: If your repo has a folder called `Edge-IIoT-ITAI3371`, you type `cd Edge-IIoT-ITAI3371` so the terminal is now inside that folder.  

- **Install dependencies** → “Download and install all the Python packages your code needs.”  
  - These packages are listed in `requirements.txt`. Running `pip install -r requirements.txt` installs them automatically.  

- **Run the main script** → “Start your program.”  
  - You type `python main.py` in the terminal, and it executes your code.  

- **Data Access** → “Where to find or simulate the data your robot uses.”  
  - Could be sensor logs, CSV files, or simulation environments like Gazebo.  

---


  
