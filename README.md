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
- **Other Libraries:** NumPy, pyttsx3 (TTS), SpeechRecognition

---

## ⚙️ Features

- 🖐️ **Sign Language Detection:**  
  Detects hand signs using webcam and classifies them using a trained TensorFlow model and MediaPipe hand tracking.

- 🔊 **Sign-to-Speech Converter:**  
  Recognized signs are converted into text and then spoken aloud using the `pyttsx3` library.

- 🗣️ **Speech-to-Text Interface:**  
  Voice input from the second user is transcribed into text using the SpeechRecognition library and displayed to the deaf/mute user.

- 🌐 **User-Friendly Web Interface:**  
  Built using Django templates, enabling smooth communication through a chat-like layout.

---

## 🧠 How It Works

1. **Gesture Input via Webcam**
   - MediaPipe detects hand landmarks.
   - TensorFlow model classifies gestures into characters or words.

2. **Text/Speech Output**
   - Recognized gestures are displayed as text and optionally voiced using TTS.

3. **Voice Input**
   - SpeechRecognition captures voice input and converts it into readable text.

4. **Communication Display**
   - A chat-like interface shows the entire interaction in real-time.

---

## 📸 Screenshots

(Add screenshots of the UI, webcam feed, chat window, etc.)

---

## 🛠️ Setup Instructions

```bash
# Clone the repository
git clone https://github.com/yourusername/two-way-deaf-communication.git
cd two-way-deaf-communication

# Create a virtual environment and activate it
python -m venv venv
source venv/bin/activate   # For Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the Django server
python manage.py runserver
