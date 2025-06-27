# 🌿 AI Garden: Predictive Irrigation & Plant Disease Classification

## 📌 Project Overview

The **AI-Powered Garden System** aims to modernize traditional gardening and small-scale agriculture using Artificial Intelligence and IoT. This project focuses on optimizing irrigation schedules, monitoring plant growth, and detecting plant diseases using real-time data and machine learning.

---

## 🎯 Mission & Vision

**Mission:**  
To contribute effectively to society through sustainable and smart garden automation.

**Vision:**  
Empowering farmers, especially the elderly and resource-constrained, with AI-driven tools for efficient farming.

**Core Values:**
- ❤️ Love of Fellow Beings  
- 🌱 Social Responsibility  
- 🏆 Pursuit of Excellence

---

## 💡 Problem Statement

### Issues:
- Water wastage due to inefficient irrigation
- Crop damage from undetected diseases

### Challenges:
- Manual monitoring and delayed interventions
- Lack of automated precision systems

### Solution:
An integrated, AI-based platform for:
- Predictive irrigation  
- Growth monitoring  
- Early disease classification

---

## 🎯 Objectives

### Primary Goal:
Build an AI system for predictive irrigation and early disease diagnosis in plants.

### Specific Objectives:
- 📊 Build an LSTM model for irrigation prediction using weather & soil data
- 🧪 Develop a CNN model for classifying plant diseases from leaf images
- 🛰️ Integrate real-time sensor data and automated irrigation response

---

## 🧠 System Components

### 🚿 Predictive Irrigation System
- **Inputs:** Weather API data, soil moisture sensors  
- **Model:** LSTM neural network  
- **Output:** Watering schedule suggestions  
- **Impact:** Reduced water usage, improved plant growth

### 🦠 Disease Detection System
- **Inputs:** Leaf and stem images  
- **Model:** Convolutional Neural Network (CNN)  
- **Output:** Type and severity of disease  
- **Impact:** Timely treatment, reduced crop loss

---

## 🏗️ System Architecture

### 🔌 Hardware
- Soil moisture sensors
- Arduino/Raspberry Pi (IoT Microcontroller)
- Automated irrigation unit (valves/pumps)
- Internet connectivity for API integration

### 🖥️ Software
- Weather API + sensor data fetch
- ML models for irrigation and classification
- Decision engine and automation scripts
- Real-time alerts and feedback loops

---

## 🧪 Model Details

### 🔹 Predictive Irrigation (LSTM)
```python
model = Sequential()
model.add(LSTM(50, return_sequences=True, input_shape=(X_train.shape[1], 1)))
model.add(LSTM(50, return_sequences=False))
model.add(Dense(1, activation='sigmoid'))
