# 🧏‍♂️ Two-Way Communication System for Deaf People

This project is an assistive communication system that bridges the gap between **deaf/mute individuals** and the **hearing population**. It enables **real-time two-way interaction** by converting **sign language gestures into text/speech** and **spoken language into text**, allowing seamless communication without a human interpreter.

---

## 🎯 Objective

- Enable **real-time communication** between deaf and hearing individuals.
- Translate **sign language gestures into voice or text output**.
- Convert **spoken words into text** for the deaf/mute person to read.
- Provide an **accessible, affordable, and scalable solution** using computer vision and AI.

---

## 🔧 Technologies Used

- **Frontend:** HTML, CSS, Bootstrap (via Django templates)
- **Backend:** Python, Django
- **Computer Vision:** OpenCV, MediaPipe
- **Machine Learning:** TensorFlow
- **Other Libraries:** NumPy, SpeechRecognition

---
# Requirements
* mediapipe 0.8.1
* OpenCV 3.4.2 or Later
* Tensorflow 2.3.0 or Later<br>tf-nightly 2.5.0.dev or later (Only when creating a TFLite for an LSTM model)
* scikit-learn 0.23.2 or Later (Only if you want to display the confusion matrix) 
* matplotlib 3.3.2 or Later (Only if you want to display the confusion matrix)
---

## ⚙️ Features

- 🖐️ **Sign Language Detection:**  
  Detects hand signs using webcam and classifies them using a trained TensorFlow model and MediaPipe hand tracking.

- 🗣️ **Speech-to-Text Interface:**  
  Voice input from the second user is transcribed into text using the SpeechRecognition library and displayed to the deaf/mute user.

- 🌐 **User-Friendly Web Interface:**  
  Built using Django templates, enabling smooth communication through a chat-like layout.

---

## 🧠 How It Works

1. **Gesture Input via Webcam**
   - MediaPipe detects hand landmarks.
   - TensorFlow model classifies gestures into characters or words.

2. **Text Output**
   - Recognized gestures are displayed as text .

3. **Voice Input**
   - SpeechRecognition captures voice input and text input converts it into readable text.

4. **Communication Display**
   - A chat-like interface shows the entire interaction in real-time.

---

## 📸 Screenshots

### 🔹 Welcome page
![Welcome page](Welcome%20page.png)

### 🔹 Login Page
![Login Page](Login%20Page.png)

### 🔹 Sign Up Page
![Sign Up Page](Sign%20Up%20Page.png)

### 🔹 Deaf to normal window
![Deaf to normal window](Deaf%20to%20normal%20window.png)

### 🔹 Hand gesture window
![Hand gesture window](Hand%20gesture%20window.png)

### 🔹 Labeled Animation
![Labeled Animation](Labeled%20Animation.png)

### 🔹 Trained Dataset
![Trained Dataset](Trained%20Dataset.png)


---

## 🛠️ Setup Instructions

```bash
# Clone the repository
git clone https://github.com/Kushalbabu10/Two_way_communication_for_Deaf_people.git
cd Two_way_communication_for_Deaf_people

# Create a virtual environment and activate it
python -m venv venv
source venv/bin/activate   # For Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the Django server
python manage.py runserver
