<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00C6FF,50:7C3AED,100:F72585&height=150&section=header&animation=fadeIn" width="100%" alt="Colorful profile header" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=34&duration=2800&pause=1200&color=8B5CF6&center=true&vCenter=true&width=960&lines=AACAAS;Electrical+Engineering+Undergraduate;AI+%7C+Computer+Vision+%7C+Robotics" alt="AACAAS — Electrical Engineering, AI, Computer Vision, and Robotics" />

<br />

<p>
  <img src="https://img.shields.io/badge/Electrical_Engineering-University_of_Moratuwa-7C3AED?style=flat-square&logo=academia&logoColor=white" alt="Electrical Engineering at the University of Moratuwa" />
  &nbsp;
  <img src="https://img.shields.io/badge/Location-Sri_Lanka-6366F1?style=flat-square&logo=googlemaps&logoColor=white" alt="Sri Lanka" />
</p>

<p>
  <a href="https://www.linkedin.com/in/muhamathu-ameer-ali/">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" />
  </a>
  &nbsp;
  <a href="https://github.com/aacaas5">
    <img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="Follow on GitHub" />
  </a>
</p>

</div>

---

I am an electrical engineering undergraduate interested in building and studying intelligent systems across both hardware and software. My work spans computer vision, reliable machine learning, multimodal visual reasoning, robotics, autonomous systems, sensing, embedded systems, and control.

I am particularly interested in understanding how intelligent systems behave under uncertainty, distribution shift, missing information, and real-world operating constraints.

---

## About Me

My electrical engineering background provides foundations in circuits, electronics, signals, sensors, control, and embedded systems. My current work extends these foundations into machine perception, learning-based systems, uncertainty quantification, robustness, autonomous systems, and intelligent decision-making.

This connection is intentional: robust perception and reliable AI require understanding both physical constraints and statistical limitations. Whether designing sensor-based data-acquisition systems or developing vision-language models that remain calibrated under evidence loss, the core challenge is building systems that behave predictably when assumptions fail.

---

## Research & Engineering Interests

### Artificial Intelligence & Perception
- Computer Vision
- Reliable & Robust Machine Learning
- Vision-Language Models / Multimodal AI
- Visual Anomaly Detection
- Confidence Calibration & Selective Prediction
- Out-of-Distribution Recognition

### Robotics & Autonomous Systems
- Autonomous Robotics & Drones
- Robot Perception & Control
- ROS 2 · ArduPilot · Gazebo
- Sensor Integration & Data Acquisition
- Autonomous Navigation & Mission Systems

### Electrical & Electronic Engineering
- Embedded Systems & Microcontrollers
- Sensors & Instrumentation
- Control Systems & Feedback
- Electronics & Signal Processing
- Data Acquisition & IoT

---

## Selected Research Projects

### Evidence-Order Calibration for Selective Visual Reasoning

**Repository:** [evidence-order-calibration-vlm](https://github.com/aacaas5/evidence-order-calibration-vlm)

Studies whether Vision-Language Model (Qwen2.5-VL) confidence tracks progressive loss of question-critical visual evidence. Uses post-hoc reliability heads trained on frozen model features with evidence-order supervision. Primary finding: Evidence-order calibration reduces violation rate (EMVR) from 0.330 to 0.303, with robust transfer to held-out blur degradation (−0.0468, 95% CI [−0.0739, −0.0199]). This represents structural-order improvement in reliability tracking, not generic confidence superiority.

**Technologies:** PyTorch · Qwen2.5-VL · GQA · Calibration · Uncertainty

---

### ShiftSplit-AD: Separating Domain Shift from Defects

**Repository:** [ShiftSplit-AD](https://github.com/aacaas5/ShiftSplit-AD)

Investigates a practical robustness problem: distinguishing real anomalies from benign domain shift using frozen DINOv2-small patch embeddings. Applies low-rank / row-sparse residual matrix decomposition to suppress nuisance feature variation. Main result: On AeBAD-S real-shift benchmark, achieves AUROC improvement of +0.0514 (0.6780 → 0.7294) with stable bootstrap intervals. However, held-out MVTec evaluation shows significant degradation, revealing the critical tradeoff: sparse filtering can suppress both domain-shift noise and genuine defect information simultaneously.

**Key Finding:** The central insight is not that the method always works, but rather that this tradeoff is fundamental and depends on whether defect and shift structure are sufficiently different.

**Technologies:** DINOv2 · PyTorch · Anomaly Detection · Robustness · Domain Adaptation

---

### Reliable Machine-Failure Prediction Under Imbalanced and Corrupted Sensor Data

**Repository:** [reliable-machine-failure-prediction-under-imbalanced-and-corrupted-sensor-data](https://github.com/aacaas5/reliable-machine-failure-prediction-under-imbalanced-and-corrupted-sensor-data)

Examines predictive maintenance as a reliability problem, not only a classification problem. Evaluates the same Random Forest model under clean data, 30% sensor noise, 30% missing measurements, and 20% training data scenarios. Clean-test recall of 82.35% deteriorates to 66.67% under noise and 50.98% under missing measurements. Includes SHAP explainability analysis to understand why some failures are detected confidently while others are missed. Demonstrates that high clean-data accuracy does not guarantee robustness to imperfect sensor and training conditions.

**Technologies:** Random Forest · SHAP · Imbalanced Data · Sensor Systems · Robustness

---

### Real-Time Object Detection Robustness Analysis

**Repository:** [real-time-object-detection-robustness-analysis](https://github.com/aacaas5/real-time-object-detection-robustness-analysis)

Evaluates YOLO26n detector behavior under controlled perturbations: confidence thresholding, brightness reduction, blur, scale, and occlusion. Finds non-monotonic detection patterns—for example, blur kernel progression shows confidence peak at kernel 11, not monotonic degradation. Demonstrates why confidence thresholds and detection counts are insufficient metrics for robustness assessment. Includes Streamlit dashboard for live webcam detection monitoring and reproducible experiment infrastructure.

**Technologies:** YOLO · OpenCV · Streamlit · Robustness Analysis · Computer Vision

---

## Selected Engineering & Autonomous Systems

### ROS 2 Autonomous Bathymetric Survey System with ArduPilot

**Repository:** [ROS2_Autonomous_Bathymetric_Survey_System_with_Ardupilot](https://github.com/RafiMAA/ROS2_Autonomous_Bathymetric_Survey_System_with_Ardupilot)

Full-stack autonomous drone system for underwater terrain mapping. Combines ROS 2 middleware, ArduPilot SITL, Gazebo simulation, and React-based ground control station. Drone autonomously navigates survey grid, classifies water vs. soil via gimbal camera (HSV thresholding), descends sonar to measure lakebed depth, and generates 3D bathymetry visualization. Demonstrates system integration across control (ArduPilot), perception (computer vision), robotics (ROS 2), and user interface (React + Three.js).

**Key Challenge:** Coordinating state machine logic, sensor timing, gimbal control, sonar depth processing, and real-time telemetry across heterogeneous middleware while maintaining mission-critical reliability.

**Technologies:** ROS 2 · ArduPilot · Gazebo · React · OpenCV · Python · C++

---

### Autonomous Smart Robot for Weed Detection and Treatment in Pots

**Repository:** [Autonomous-Smart-Robot-for-Weed-Detection-and-Treatment-in-Pots](https://github.com/aacaas5/Autonomous-Smart-Robot-for-Weed-Detection-and-Treatment-in-Pots)

Integrated AI/robotics/embedded platform combining Python orchestration, Arduino firmware, LabVIEW data acquisition, and computer vision. Four-wheel mobile robot autonomously moves between potted plants, uses IR tape sensor for arrival detection, positions camera via servo gimbal, detects weeds using Inference SDK model, analyzes plant health via HSV color masks, and uploads scan results. End-to-end system demonstrates perception-to-action pipeline, sensor integration, embedded control, DAQ monitoring, and multi-technology communication (TCP/IP, serial, HTTP).

**Technical Scope:** Motor control · Servo gimbal · IR sensing · Camera capture · Vision inference · Condition analysis · LabVIEW DAQ · Web integration

**Technologies:** Python · Arduino · LabVIEW · OpenCV · Computer Vision · Embedded Systems · DAQ

---

## How I Approach Problems

**Problem** → **Hypothesis** → **Experimental Design** → **Implementation** → **Quantitative Evaluation** → **Failure Analysis** → **Reproducibility**

I increasingly structure projects as small experimental studies rather than only implementation demos. This means asking clear research questions, controlling variables, reporting negative or mixed findings honestly, and ensuring reproducibility through documented methods and artifact preservation.

---

## Technical Toolbox

### Languages

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,cpp,matlab&theme=dark" alt="Python, C++, and MATLAB" />
</p>

### AI & Computer Vision

<p align="center">
  <img src="https://skillicons.dev/icons?i=pytorch,opencv,sklearn&theme=dark" alt="PyTorch, OpenCV, and scikit-learn" />
</p>

NumPy · pandas · Qwen2.5-VL · DINOv2 · YOLO · Streamlit

### Robotics & Autonomous Systems

<p align="center">
  <img src="https://skillicons.dev/icons?i=ros&theme=dark" alt="ROS" />
</p>

ArduPilot · Gazebo · MAVROS · rosbridge

### Embedded & Electronics

<p align="center">
  <img src="https://skillicons.dev/icons?i=arduino&theme=dark" alt="Arduino" />
</p>

Sensors · Data Acquisition · Microcontrollers · DAQ Systems

### Engineering & Simulation
Simulink · LabVIEW · Signal Processing

### Development

<p align="center">
  <img src="https://skillicons.dev/icons?i=git,github,vscode&theme=dark" alt="Git, GitHub, and Visual Studio Code" />
</p>

Jupyter Notebooks

---

## Current Focus

Exploring reliability in visual intelligence—particularly how models behave under missing evidence, domain shift, out-of-distribution inputs, and uncertainty. Continuing to build autonomous perception and engineering systems that integrate sensors, embedded control, and learning-based reasoning into coherent end-to-end platforms.

---

## Connect

**GitHub:** [github.com/aacaas5](https://github.com/aacaas5)

**LinkedIn:** [linkedin.com/in/muhamathu-ameer-ali](https://linkedin.com/in/muhamathu-ameer-ali)

<!-- **Email:** [your.email@example.com](mailto:your.email@example.com) -->

---

*Last updated: August 30, 2026*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F72585,50:7C3AED,100:00C6FF&height=120&section=footer" width="100%" alt="Colorful profile footer" />
