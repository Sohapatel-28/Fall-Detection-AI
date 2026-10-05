# Fall-Detection-AI
AI-Powered Elderly Fall Detection System Machine Learning and Deep Learning – FA-2  Student: Soha Grade: 12 IBCP CRS: Artificial Intelligence School: Udgam School for Children

#  AI-Powered Elderly Fall Detection System

### Machine Learning & Deep Learning | Computer Vision | Pose Estimation | Real-Time Monitoring

An **AI-powered elderly fall detection and activity monitoring system** developed as part of the **Artificial Intelligence Career-Related Study (CRS)**.

The project combines **Computer Vision, Pose Estimation, Machine Learning, Deep Learning, and Streamlit** to analyse human posture and movement, classify activities, detect potential falls, generate emergency alerts, and provide an interactive monitoring dashboard.

---

##  Project Overview

Falls are a major safety concern for elderly individuals, particularly when they are alone or require continuous monitoring.

This project aims to develop an AI-assisted monitoring system that can identify different human activities and detect potentially dangerous fall incidents.

The system supports **three major detection modes**:

### 🖼️ Image Detection
Analyse an uploaded image and identify the person's activity and posture.

### 🎥 Video Detection
Upload a video and analyse movement across frames to identify activities and potential falls.

### 📹 Live Monitoring & Real-Time Detection
Use live camera monitoring to continuously analyse human movement and detect potential fall incidents in real time.

The complete system is integrated into an interactive **Streamlit dashboard**.

---

#  Key Features

## 🖼️ 1. Image-Based Fall Detection

The image detection module allows the user to upload an image for AI analysis.

The system analyses the person's posture and predicts the detected activity.

### Features include:

- Human detection
- Pose estimation
- Body landmark analysis
- Activity classification
- Fall detection
- Prediction confidence
- Pose visualization
- Emergency warning for detected falls

### Workflow

```text
Upload Image
     ↓
Human Detection
     ↓
Pose Estimation
     ↓
Posture Analysis
     ↓
Activity Classification
     ↓
Fall / Normal Activity
     ↓
Prediction + Confidence
```

---

#  2. Video-Based Fall Detection

The video detection module allows users to upload a video and analyse human movement.

The system processes the video and analyses the person's posture and activity across frames.

### Features include:

- Video upload
- Frame-by-frame analysis
- Human pose detection
- Activity classification
- Fall detection
- Prediction confidence
- Pose visualization
- Fall alerts
- Monitoring results

### Workflow

```text
Upload Video
     ↓
Video Processing
     ↓
Frame Analysis
     ↓
Pose Estimation
     ↓
Activity Classification
     ↓
Fall Detection
     ↓
Results + Alert
```

---

#  3. Live Monitoring & Real-Time Fall Detection

## 🔴 REAL-TIME MONITORING

A major feature of this project is **live monitoring and real-time fall detection**.

The system can monitor a live camera feed and continuously analyse human posture and movement.

The incoming frames are processed by the AI system to identify the current activity.

If a potential fall is detected, the system highlights the incident and generates an emergency warning.

### Live monitoring provides:

- 📹 Live camera monitoring
- 🧍 Real-time pose estimation
- 🤖 Real-time activity classification
- 🚨 Real-time fall detection
- ⚠️ Emergency alerts
- 📊 Monitoring information
- 📈 Prediction confidence

This demonstrates how computer vision and AI can be applied to continuous elderly safety monitoring.

---

#  4. Emergency Fall Alert System

When the system identifies a potential fall, an emergency warning is displayed on the dashboard.

### Example:

```text
🚨 FALL DETECTED

Potential fall incident detected.
Immediate attention may be required.
```

The alert system is designed to make potentially dangerous events clearly visible to a caregiver or monitoring user.

The assignment specifically requires warning messages or emergency notifications when a fall is detected.

---

# 🧍 5. Human Pose Estimation

Pose estimation is used to understand human posture and body movement.

The system analyses body landmarks such as:

- Shoulders
- Elbows
- Hips
- Knees
- Ankles

These keypoints help the AI understand body posture and movement patterns.

Pose estimation is an important part of the fall detection pipeline because a fall can involve a significant change in body orientation and posture.

The assignment identifies **MediaPipe Pose, YOLOv8 Pose Estimation, and OpenPose** as suitable pose-estimation approaches.

---

#  6. Activity Classification

The AI system classifies different human activities.

### Activity Classes

| Activity | Description |
|---|---|
| 🚨 Fall Detected | Potential fall incident |
| 🚶 Walking | Person is walking |
| 🪑 Sitting | Person is sitting |
| 🧍 Standing | Person is standing |
| ✅ Normal Activity | Normal movement/activity |

The activity classification system analyses posture and movement patterns to determine the most likely activity.

---

#  7. Prediction Confidence

For each prediction, the system provides a confidence score.

This allows the user to see:

```text
Predicted Activity
        +
Confidence Score
```

The confidence information provides additional context when interpreting the AI prediction.

---

# 📈 8. Monitoring Analytics

The Streamlit dashboard provides monitoring information and activity statistics.

### Dashboard information includes:

- Total activities detected
- Fall detected count
- Normal activity count
- Prediction confidence
- Activity distribution
- Pose visualization
- Emergency alerts

The FA-2 requirements specifically identify these monitoring and dashboard outputs.

---

# 🧠 AI Detection Workflow

```text
                   INPUT
                     │
          ┌──────────┼──────────┐
          │          │          │
        IMAGE      VIDEO    LIVE CAMERA
          │          │          │
          └──────────┼──────────┘
                     ↓
             HUMAN DETECTION
                     ↓
              POSE ESTIMATION
                     ↓
          BODY LANDMARK ANALYSIS
                     ↓
          ACTIVITY CLASSIFICATION
                     ↓
             FALL DETECTION
                     ↓
          ┌──────────┴──────────┐
          │                     │
    NORMAL ACTIVITY        FALL DETECTED
          │                     │
          ↓                     ↓
     MONITORING               ALERT
          │                     │
          └──────────┬──────────┘
                     ↓
          CONFIDENCE + ANALYTICS
                     ↓
            STREAMLIT DASHBOARD
```

---

# 🧪 Model Training & Evaluation

The project includes a model training and evaluation pipeline.

The dataset is divided into:

- **70% Training Set**
- **15% Validation Set**
- **15% Testing Set**

This follows the dataset distribution specified in the assignment brief.

## Evaluation Metrics

The model is evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-Score**

The project also includes:

- Confusion Matrix
- Training curves
- Accuracy graph
- Loss graph
- Prediction outputs

These metrics are required to evaluate the performance of the fall detection and activity classification system.

---

#  Confusion Matrix

The confusion matrix is used to analyse classification performance.

It helps identify:

- Correct fall detections
- False fall detections
- Correct activity classifications
- Misclassified activities

This provides a clearer understanding of the strengths and limitations of the trained model.

---

#  Streamlit Web Application

The trained AI model is integrated into an interactive **Streamlit application**.

The application provides a user-friendly interface for accessing the different detection modes.

## Available Modes

###  Image Detection

Upload an image → Analyse → Predict activity → Display result

###  Video Detection

Upload a video → Process frames → Analyse movement → Detect activity/fall

###  Live Monitoring

Start camera → Analyse live frames → Classify activity → Detect fall → Generate alert

The assignment requires the final healthcare monitoring application to be deployed using Streamlit Cloud.

---

#  Application Screenshots

##  Main Dashboard

The main Streamlit interface provides access to the AI-powered monitoring features.

**Screenshot:**  
_Add working application screenshot here._

---

##  Image Detection

The image detection interface allows users to upload an image and receive an AI-based activity/fall prediction.

**Screenshot:**  
_Add image detection screenshot here._

---

##  Video Detection

The video detection interface analyses uploaded video content and identifies activities and potential fall events.

**Screenshot:**  
_Add video detection screenshot here._

---

##  Live Monitoring

The live monitoring interface provides real-time analysis of camera input.

**Screenshot:**  
_Add live monitoring screenshot here._

---

##  Fall Alert

The application highlights a detected fall and displays an emergency warning.

**Screenshot:**  
_Add fall alert screenshot here._

---

##  Pose Detection

The pose estimation output displays human body landmarks used for posture and movement analysis.

**Screenshot:**  
_Add pose detection screenshot here._

---

## Monitoring Analytics

The dashboard displays activity statistics, prediction confidence and monitoring information.

**Screenshot:**  
_Add analytics screenshot here._

---

#  Technologies Used

## Programming Language

- Python

## AI & Computer Vision

- Machine Learning
- Deep Learning
- Computer Vision
- Pose Estimation
- Activity Classification

## Libraries & Frameworks

- TensorFlow / Keras
- OpenCV
- MediaPipe
- Scikit-learn
- Streamlit

The assignment recommends Python-based development environments and these AI/computer-vision libraries.

---

#  Project Structure

```text
Fall-Detection-AI/
│
├── app.py
├── train_model.py
├── evaluate_model.py
├── test_setup.py
├── extract_features.py
├── split_data.py
│
├── fall_detection_model.keras
├── label_classes.txt
│
├── train_data.csv
├── test_data.csv
├── val_data.csv
├── pose_data.csv
│
├── training_history.csv
├── evaluation_report.txt
│
├── confusion_matrix.png
├── training_curves.png
│
├── requirements.txt
│
└── README.md
```

---

#  Project Objectives

The main objectives of this project are to:

1. Develop an AI-powered elderly fall detection system.
2. Detect human posture and body movement.
3. Classify human activities.
4. Detect potentially dangerous falls.
5. Generate emergency alerts.
6. Analyse uploaded images.
7. Analyse uploaded videos.
8. Perform live monitoring and real-time detection.
9. Display prediction confidence.
10. Provide monitoring analytics.
11. Evaluate the trained model.
12. Deploy the solution through Streamlit.

---

#  Real-World Application

The system demonstrates how AI and computer vision can support elderly safety monitoring.

Potential applications include:

- Elderly care centres
- Healthcare monitoring environments
- Hospitals
- Caregiver monitoring
- Assisted living environments
- Home-based elderly monitoring

The system is intended as an **AI-assisted monitoring tool** and should not be considered a replacement for professional medical or emergency services.

---

#  Limitations

Real-world fall detection can be affected by different environmental and human factors.

Potential challenges include:

- Lighting variation
- Camera angle differences
- Partial body occlusion
- Similar body postures
- False fall detections
- Limited training data
- Different backgrounds and environments

These challenges are also identified in the FA-2 assignment requirements.

---

  Future Improvements

Possible future improvements include:

- Improved performance in low-light environments
- Improved elderly posture recognition
- Reduction of false alerts
- Larger and more diverse datasets
- Improved pose estimation
- Support for real-time CCTV feeds
- Improved activity recognition
- Periodic model retraining
- Enhanced monitoring analytics

These areas are specifically identified as possible improvements in the assignment brief.

---

  Project Demonstration

The final demonstration of the project covers:

- Project overview
- Dataset explanation
- Pose estimation outputs
- Model predictions
- Image detection
- Video detection
- Live monitoring
- Streamlit dashboard
- Evaluation metrics
- Confusion matrix
- Fall alert demonstration

The assignment requires the final evidence to include a project video and deployed Streamlit link, together with these demonstration components.

---

#  Student Information

**Student:** Soha  
**Grade:** 12 IBCP  
**Career-Related Study:** Artificial Intelligence  
**School:** Udgam School for Children, Ahmedabad  

**Course:** Machine Learning and Deep Learning  
**Assessment:** Formative Assessment 2  

### Assignment Title

**Developing an AI-Powered Elderly Fall Detection System using Machine Learning and Deep Learning**

---

#  Academic Context

This project was developed as part of the **Artificial Intelligence Career-Related Study (CRS)** and the **Machine Learning and Deep Learning – Formative Assessment 2**.

The project builds upon the earlier analysis and planning work and focuses on the implementation, training, evaluation and deployment of an AI-powered healthcare monitoring system.

---

# 📌 Project Files & Demonstration Note

Due to the **large size of the complete project files, datasets, trained models, and associated resources**, the entire set of project files has not been uploaded to this repository/submission space.

The repository therefore focuses on the **project documentation, implementation structure, results and demonstration of the working application**.

The **working application screenshots provided with the project demonstrate the actual implemented system and its major features**, including:

- 🖼️ Image Detection
- 🎥 Video Detection
- 📹 Live Monitoring
- 🧍 Pose Estimation
- 🤖 Activity Classification
- 🚨 Fall Detection
- ⚠️ Emergency Alerts
- 📊 Monitoring Analytics
- 📈 Prediction Confidence
- 🌐 Streamlit Dashboard

The screenshots serve as visual evidence of the working application and demonstrate how the implemented AI system operates across its different monitoring and detection features.

---

# ⭐ Project Highlights

### 🖼️ IMAGE DETECTION
Upload an image and analyse human posture and activity using AI.

### 🎥 VIDEO DETECTION
Upload and analyse video frames to identify activities and potential falls.

### 📹 LIVE MONITORING
Perform continuous real-time monitoring using live camera input.

### 🚨 FALL DETECTION
Identify potential fall incidents and highlight them immediately.

### ⚠️ EMERGENCY ALERTS
Generate visible warnings when a potential fall is detected.

### 🧍 POSE ESTIMATION
Analyse human body landmarks and posture.

### 🤖 ACTIVITY CLASSIFICATION
Identify walking, sitting, standing, normal activity and falling.

### 📊 MONITORING ANALYTICS
Display activity counts, confidence scores and monitoring information.

### 🌐 STREAMLIT APPLICATION
Provide an interactive and user-friendly healthcare monitoring interface.

---

## 🚀 Final Project

**AI-Powered Elderly Fall Detection System**

**Machine Learning + Deep Learning + Computer Vision + Pose Estimation + Streamlit**
