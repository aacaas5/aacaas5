<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00C6FF,50:7C3AED,100:F72585&height=150&section=header&animation=fadeIn" width="100%" alt="Profile header" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=34&duration=2800&pause=1200&color=8B5CF6&center=true&vCenter=true&width=960&lines=AACAAS;Electrical+Engineering+Undergraduate;Reliable+AI+%7C+Computer+Vision+%7C+Robotics" alt="AACAAS - Electrical Engineering, Reliable AI, Computer Vision, and Robotics" />

<p>
  <img src="https://img.shields.io/badge/Electrical_Engineering-University_of_Moratuwa-7C3AED?style=flat-square" alt="Electrical Engineering at the University of Moratuwa" />
  &nbsp;
  <img src="https://img.shields.io/badge/Location-Sri_Lanka-6366F1?style=flat-square&logo=googlemaps&logoColor=white" alt="Sri Lanka" />
</p>

<p>
  <a href="https://www.linkedin.com/in/aacaas-muhamathu-023765430/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="Connect on LinkedIn" /></a>
  &nbsp;
  <a href="mailto:aacaas05@gmail.com"><img src="https://img.shields.io/badge/Email-Reach_Out-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Send an email" /></a>
  &nbsp;
  <a href="https://github.com/aacaas5?tab=repositories"><img src="https://img.shields.io/badge/GitHub-Explore_My_Work-181717?style=for-the-badge&logo=github&logoColor=white" alt="Explore my repositories" /></a>
</p>

</div>

## Hello, I am AACAAS

I am an Electrical Engineering undergraduate at the University of Moratuwa building intelligent systems across **AI, computer vision, robotics, sensing, embedded systems, and control**.

My main research interest is **reliable intelligence**: understanding how models and autonomous systems behave when evidence is missing, inputs shift, sensors are corrupted, or real-world assumptions fail. I turn those questions into reproducible experiments and end-to-end engineering systems.

> **Current focus:** reliable visual reasoning, uncertainty and calibration, out-of-distribution detection, autonomous perception, and sensor-to-action systems.

---

## Featured Work

### 1. Evidence-Order Calibration for Selective Visual Reasoning

[![Repository](https://img.shields.io/badge/View_Repository-evidence--order--calibration--vlm-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/evidence-order-calibration-vlm)

A paper-backed study of whether a Vision-Language Model's confidence tracks the progressive loss of question-critical visual evidence. I trained lightweight reliability heads over a frozen Qwen2.5-VL model and introduced evidence-order supervision to improve the structure of confidence trajectories.

- Reduced Evidence Monotonicity Violation Rate from **0.330 to 0.303** over critical-mask trajectories.
- Transferred the ordering improvement to a held-out local-blur degradation: **-0.0468 EMVR difference**, 95% CI `[-0.0739, -0.0199]`.
- Includes the manuscript, frozen benchmark artifacts, staged experiments, ablations, controls, and reproducibility scripts.

`Qwen2.5-VL` `PyTorch` `GQA` `Calibration` `Uncertainty` `Selective Prediction`

---

### 2. ShiftSplit-AD: Separating Domain Shift from Defects

[![Repository](https://img.shields.io/badge/View_Repository-ShiftSplit--AD-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/ShiftSplit-AD)

A robustness study that asks whether benign domain shift can be separated from genuine industrial defects in frozen DINOv2 feature residuals. The method applies low-rank and row-sparse decomposition, then evaluates both its gains and its failure modes.

- Improved AeBAD-S real-shift AUROC from **0.6780 to 0.7294**.
- Tested transfer on MVTec and documented an important limitation: filtering nuisance variation can also suppress genuine defect evidence.
- Emphasizes controlled evaluation, bootstrap uncertainty, negative findings, and reproducible analysis.

`DINOv2` `PyTorch` `Anomaly Detection` `Domain Shift` `Robustness`

---

### 3. Autonomous Bathymetric Survey Drone

[![Repository](https://img.shields.io/badge/View_Repository-ROS_2_Bathymetric_Drone-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/ROS2_Autonomous_Bathymetric_Survey_System_with_Ardupilot)

A full-stack autonomous survey system that combines ROS 2, ArduPilot SITL, Gazebo, computer vision, sonar sensing, and a React ground-control station. The drone follows a survey grid, distinguishes water from soil, measures depth, estimates volume, and produces interactive 3D bathymetry.

- Autonomous state-machine mission from waypoint planning through return-to-launch.
- Real-time telemetry and mission control through ROS-WebSocket integration.
- Interactive Three.js visualization of surveyed underwater terrain.

`ROS 2` `ArduPilot` `Gazebo` `MAVROS` `OpenCV` `React` `Three.js`

---

### 4. Autonomous Smart Robot for Weed Detection and Treatment

[![Repository](https://img.shields.io/badge/View_Repository-Smart_Garden_Robot-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/Autonomous-Smart-Robot-for-Weed-Detection-and-Treatment-in-Pots)

An integrated AI, robotics, and embedded platform that moves between potted plants, detects weeds, evaluates plant condition, and reports scan results. It connects camera-based inference with motor control, servo positioning, IR sensing, LabVIEW data acquisition, and web telemetry.

- End-to-end perception-to-action workflow across Python and Arduino.
- Multi-sensor acquisition and monitoring through LabVIEW.
- Serial, TCP/IP, and HTTP communication across the system.

`Python` `Arduino` `LabVIEW` `OpenCV` `Computer Vision` `DAQ`

---

### 5. Dual-Signal OOD Gating for Skin-Cancer Classification

[![Repository](https://img.shields.io/badge/View_Repository-Dual--Signal_OOD_Gating-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/dual-signal-ood-gating-for-skin-cancer-detection)

A research prototype for open-set skin-lesion classification that combines a ResNet50 classifier with two rejection signals: ViT embedding distance and Energy + ReAct scoring. A Flask application provides both browser-based uploads and a JSON prediction API.

- Classifies three lesion categories while rejecting unsupported inputs before classification.
- Exposes gate scores, thresholds, pass/fail states, confidence, and class probabilities.
- Includes model research, OOD benchmarking, exported artifacts, technical documentation, and an application interface.

`ResNet50` `Vision Transformer` `Energy + ReAct` `PyTorch` `Flask` `OOD Detection`

> Research use only; this prototype is not a validated medical device.

---

### 6. Reliable Machine-Failure Prediction

[![Repository](https://img.shields.io/badge/View_Repository-Reliable_Machine_Failure_Prediction-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/reliable-machine-failure-prediction-under-imbalanced-and-corrupted-sensor-data)

A predictive-maintenance study that treats machine-failure classification as a reliability problem. The same Random Forest model is evaluated under class imbalance, sensor noise, missing measurements, and limited training data.

- Compares clean performance with controlled corruption and data-scarcity scenarios.
- Shows recall falling from **82.35%** on clean data to **66.67%** with sensor noise and **50.98%** with missing measurements.
- Uses SHAP analysis to explain confident detections and missed failures.

`Random Forest` `SHAP` `Sensor Data` `Imbalanced Learning` `Robustness`

---

### 7. Real-Time Object-Detection Robustness Analysis

[![Repository](https://img.shields.io/badge/View_Repository-Object_Detection_Robustness-181717?style=for-the-badge&logo=github)](https://github.com/aacaas5/real-time-object-detection-robustness-analysis)

A YOLO-based real-time detection system and controlled study of how detector behavior changes under low light, blur, scale, occlusion, and confidence-threshold variation.

- Tracks confidence, detection count, FPS, and latency during live webcam inference.
- Reveals non-monotonic detector responses that simple threshold metrics can miss.
- Includes reproducible experiment infrastructure and an interactive Streamlit dashboard.

`YOLO` `OpenCV` `Streamlit` `Computer Vision` `Robustness Analysis`

---

## More Projects

Each title links directly to its repository.

| Project | What it demonstrates | Focus |
|---|---|---|
| [Visual Representation Analysis with CNNs](https://github.com/aacaas5/visual-representation-analysis-cnn) | Explores CIFAR-10 representations using feature maps, PCA, confidence analysis, confusion matrices, and Grad-CAM. | PyTorch, interpretability, CNNs |
| [Real-Time Face Recognition and Embedding Matching](https://github.com/aacaas5/real-time-face-recognition-embedding-matching) | Local enrollment, embedding-based matching, threshold rejection, evaluation infrastructure, and runtime benchmarking. | Face embeddings, OpenCV, evaluation |
| [Advanced Light Intensity Indicator](https://github.com/aacaas5/The-Advanced-Light-Intensity-Indicator-ALII-Module) | Hardware-only light monitoring with an LDR, noise filtering, stability control, timing logic, and dual seven-segment displays. | Digital electronics, instrumentation |
| [Dual-Axis Solar Tracking System](https://github.com/aacaas5/dual-axis-solar-tracking-system) | Mechanical design, electronics, embedded control, and MATLAB/Simulink simulation for automatic PV panel orientation. | Control, CAD, renewable energy |
| [Handwritten Digit Recognition](https://github.com/aacaas5/handwritten-digit-recognition) | A fully connected PyTorch neural network trained and evaluated on MNIST. | Deep-learning fundamentals |
| [Gradient Descent Optimization Lab](https://github.com/aacaas5/gradient-descent-optimization-lab) | A focused exploration of gradient-based optimization. | Optimization, machine learning |
| [Smart Garden Monitor](https://github.com/aacaas5/smart_garden_monitor) | A TypeScript-based interface for smart-garden monitoring. | TypeScript, web telemetry |

<div align="center">
  <a href="https://github.com/aacaas5?tab=repositories"><img src="https://img.shields.io/badge/Explore_All_14_Repositories-7C3AED?style=for-the-badge&logo=github&logoColor=white" alt="Explore all repositories" /></a>
</div>

---

## Technical Toolkit

### Languages

<p align="center">
  <img src="https://skillicons.dev/icons?i=py,cpp,matlab,js,ts&theme=dark" alt="Python, C++, MATLAB, JavaScript, and TypeScript" />
</p>

### AI, Machine Learning & Computer Vision

<p align="center">
  <img src="https://skillicons.dev/icons?i=pytorch,opencv,sklearn&theme=dark" alt="PyTorch, OpenCV, and scikit-learn" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
  <img src="https://img.shields.io/badge/pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="pandas" />
  <img src="https://img.shields.io/badge/YOLO-111F68?style=for-the-badge&logo=yolo&logoColor=white" alt="YOLO" />
  <img src="https://img.shields.io/badge/Qwen2.5--VL-615CED?style=for-the-badge" alt="Qwen2.5-VL" />
  <img src="https://img.shields.io/badge/DINOv2-0467DF?style=for-the-badge" alt="DINOv2" />
</p>

### Web Applications & Visualization

<p align="center">
  <img src="https://skillicons.dev/icons?i=html,css,js,ts,react,threejs,flask&theme=dark" alt="HTML, CSS, JavaScript, TypeScript, React, Three.js, and Flask" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />
</p>

### Robotics, Autonomous Systems & Embedded Engineering

<p align="center">
  <img src="https://skillicons.dev/icons?i=ros,arduino&theme=dark" alt="ROS and Arduino" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/ArduPilot-0D7FBD?style=for-the-badge&logo=ardupilot&logoColor=white" alt="ArduPilot" />
  <img src="https://img.shields.io/badge/Gazebo-F58113?style=for-the-badge&logo=gazebo&logoColor=white" alt="Gazebo" />
  <img src="https://img.shields.io/badge/MAVROS-334155?style=for-the-badge" alt="MAVROS" />
  <img src="https://img.shields.io/badge/Sensors-0891B2?style=for-the-badge" alt="Sensors" />
  <img src="https://img.shields.io/badge/Data_Acquisition-0F766E?style=for-the-badge" alt="Data Acquisition" />
</p>

### Power Systems, CAD & Engineering Simulation

<p align="center">
  <img src="https://skillicons.dev/icons?i=autocad,matlab&theme=dark" alt="AutoCAD and MATLAB" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PSCAD-005DAA?style=for-the-badge" alt="PSCAD" />
  <img src="https://img.shields.io/badge/PSS%C2%AE%20E-1F4E79?style=for-the-badge" alt="PSS/E" />
  <img src="https://img.shields.io/badge/SolidWorks-E2231A?style=for-the-badge" alt="SolidWorks" />
  <img src="https://img.shields.io/badge/Simulink-F59E0B?style=for-the-badge" alt="Simulink" />
  <img src="https://img.shields.io/badge/LabVIEW-FFDB00?style=for-the-badge&logo=labview&logoColor=black" alt="LabVIEW" />
</p>

### Development Tools

<p align="center">
  <img src="https://skillicons.dev/icons?i=git,github,vscode&theme=dark" alt="Git, GitHub, and Visual Studio Code" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter Notebooks" />
</p>

---

## How I Work

`Problem` -> `Hypothesis` -> `Experimental Design` -> `Implementation` -> `Quantitative Evaluation` -> `Failure Analysis` -> `Reproducibility`

I approach projects as engineering systems and small experimental studies: define the question, control the variables, measure the outcome, document limitations honestly, and preserve enough detail for the work to be reproduced.

---

## Let us Connect

- **GitHub:** [github.com/aacaas5](https://github.com/aacaas5)
- **LinkedIn:** [linkedin.com/in/aacaas-muhamathu-023765430](https://www.linkedin.com/in/aacaas-muhamathu-023765430/)
- **Email:** [aacaas05@gmail.com](mailto:aacaas05@gmail.com)

<div align="center">

*Open to research collaboration, engineering projects, and conversations about reliable AI, computer vision, and autonomous systems.*

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F72585,50:7C3AED,100:00C6FF&height=120&section=footer" width="100%" alt="Profile footer" />

</div>
