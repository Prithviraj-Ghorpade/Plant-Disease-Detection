# 🪴 Plant Disease Detection

This project is designed to help farmers and agricultural experts detect plant diseases using machine learning while also providing real-time weather information. It integrates a convolutional neural network (CNN) model, OpenWeather API for weather data, and location services to deliver insights and recommendations.

---

## Table of Contents
- 🌟 [Features](#features)
- 🛠️ [Tech Stack](#tech-stack)
- 📊 [Dataset](#dataset)
- 🏗️ [System Architecture](#system-architecture)
- ⚙️ [Setup Instructions](#setup-instructions)
- 🚀 [Usage](#usage)
- 📂 [Project Structure](#project-structure)
- 🧪 [Results](#results)
- 📰 [Publications](#publications)
- 👥 [Contributors](#contributors)

---

## 🌟 Features
- **Plant Disease Detection**: A trained CNN model identifies diseases from plant leaf images.
- **Weather Information**: Real-time weather updates via the OpenWeather API.
- **Location-Based Services**: Location-specific weather and prediction data.
- **User-Friendly App**: Simple Android application interface for disease prediction and weather updates.

---

## 🛠️ Tech Stack
- **Frontend**: Android (Java and Kotlin)
- **Backend**: Python, TensorFlow
- **Machine Learning**: Convolutional Neural Network (`Plant_model.h5`)
- **API Integration**: OpenWeather API
- **Tools**: Android Studio, Python Libraries, Firebase

---

## 📊 Dataset
The dataset includes plant leaf images with labeled diseases, sourced from platforms like [Kaggle](https://www.kaggle.com/). It contains classes for various plant diseases and healthy leaves.

---

## 🏗️ System Architecture
1. **Image Input**: Users capture or upload an image of a plant leaf through the app.
2. **Disease Detection**: The image is analyzed by the CNN model for disease prediction.
3. **Weather Integration**: Fetches real-time weather data based on the user's location.
4. **Display Results**: Outputs disease diagnosis and weather information.

---

## ⚙️ Setup Instructions

### Prerequisites
- Android Studio installed on your system.
- Python 3.8 or above installed.
- OpenWeather API Key (Sign up at [OpenWeather](https://openweathermap.org/)).
  
---

## 🚀 Usage
1. Build and run the Android app on your device or emulator.
2. Upload or take a photo of a plant leaf.
3. View the prediction result (disease diagnosis) on the app.
4. Check the weather details for the current or specified location.

---

## 📂 Project Structure

### Crop Disease Project (Android Application)
- ├── .idea ------------------------------------------------- Android Studio project configuration files
- ├── app
- │   ├── src
- │   │   ├── androidTest/java/com/example/crop_disease
- │   │   │   └── ExampleInstrumentedTest.kt ---------------- Instrumentation tests
- │   │   ├── main
- │   │   │   ├──java/com/example/crop_disease
- │   │   │   │   ├── CropPrediction.kt -------------------------- Prediction logic and ML model integration
- │   │   │   │   ├── MainActivity.kt ----------------------------- Main activity (app entry point)
- │   │   │   │   ├── Register.kt ---------------------------------- User registration activity
- │   │   │   │   ├── detection.java ------------------------------ Disease detection implementation
- │   │   │   │   ├── home.java ---------------------------------- Home screen activity
- │   │   │   │   ├── location.kt ---------------------------------- Location-based service handling
- │   │   │   │   ├── notify.kt ------------------------------------- Notification handling logic
- │   │   │   │   ├── weather.java -------------------------------- Weather API integration
- │   │   │   ├── res --------------------------------------------- Android resources folder
- │   │   │   │   ├── drawable ------------------------------------ Graphics and images
- │   │   │   │   ├── layout --------------------------------------- XML layouts for UI design
- │   │   │   │   ├── mipmap ------------------------------------- App icons for different screen densities
- │   │   │   │   ├── values --------------------------------------- Strings, themes, colors, and styles
- │   │   │   │   ├── xml ------------------------------------------ Configuration files (e.g., network security)
- │   │   │   ├── ml
- │   │   │   │   ├── model.tflite ---------------------------------- Pre-trained TensorFlow Lite model
- │   │   │   ├── AndroidManifest.xml -------------------------- Android app configuration and permissions
- │   ├── build.gradle ---------------------------------------- Gradle build configuration
- │   ├── google-services.json ------------------------------- Firebase configuration
- │   ├── proguard-rules.pro --------------------------------- Rules for code obfuscation

### Test code
- ├── CNNModelp.py --------------------------------------- Python script for training the CNN model
- ├── GUI_Master_old.py ------------------------------------ Prototype GUI for testing the model
- ├── Plant_model.h5 --------------------------------------- Trained CNN model (Keras format)
- ├── accuracy.jpg ------------------------------------------- Accuracy graph for model training
- ├── loss.jpg ------------------------------------------------ Loss graph for model training
- ├── test_set ------------------------------------------------ Test data
- │   ├── 0 ----------------------------------------------------- Category 0 
- │   ├── 1 ----------------------------------------------------- Category 1 
- │   ├── 2 ----------------------------------------------------- Category 2 
- ├── training_set -------------------------------------------- Training data
- │   ├── 0 ----------------------------------------------------- Category 0 
- │   ├── 1 ----------------------------------------------------- Category 1 
- │   ├── 2 ----------------------------------------------------- Category 2 
- ├── test_set.zip --------------------------------------------- Zipped test set for easy sharing

---

## 🧪 Results
- Model Accuracy: Achieved Training Accuracy of 99.67% and Testing Accuracy of 33.11%
- Integration: Successfully integrated disease prediction, weather, location, and crop prediction using soil type data into a single application.

---

## 📰 Publications
1. **SSRN (Social Science Research Network)**: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4716094
2. **IJIRCCE (International Journal of Innovative Research in Computer and Communication Engineering)**: https://ijircce.com/admin/main/storage/app/pdf/F1YEFPg8egBe72LLxwUa4EWpFJdXlBbDtp2eVNLp.pdf

---

## 👥 Contributors
1. Prithviraj Ghorpade
2. Vaibhav Lahase
3. Abhishek Linge

