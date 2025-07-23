 #Real-Time Virtual Keyboard Using Hand Gestures
 
This project is a gesture-controlled virtual keyboard built using OpenCV, MediaPipe, and Python. It enables real-time, touchless typing by detecting hand and finger movements via a webcam — simulating key presses on a virtual keyboard displayed on the screen.

📌 Objective
To design a deep learning-powered, contactless keyboard interface that allows users to type using only hand gestures — useful for accessibility tools, interactive kiosks, and hands-free applications.

⚙️ How It Works
Hand Detection:
MediaPipe's hand tracking module detects and tracks 21 hand landmarks from the webcam stream in real time.

Virtual Keyboard Layout:
A full QWERTY keyboard layout (with numbers, symbols, and function keys like CAPS, SPACE, DEL, ENTER) is rendered using OpenCV.

Gesture Mapping:
The fingertip position (index finger) is used to identify which key the user is hovering over.

Click Logic:
A cooldown mechanism ensures that a key is only triggered once per hover, preventing false key presses.

Simulated Typing:
Keys are simulated using pyautogui, and a new Notepad window is opened using subprocess for real-time text entry.

🧰 Libraries & Tools Used
Library	Purpose
OpenCV	Video capture, keyboard rendering, UI
MediaPipe	Real-time hand landmark detection
NumPy	Coordinate and mathematical operations
math	Calculations for finger position logic
pyautogui	Simulating keyboard input into Notepad
subprocess	Launching external Notepad application

🔑 Features
✅ Real-time hand tracking with MediaPipe

✅ Full keyboard layout (letters, numbers, symbols, controls)

✅ Caps Lock, Backspace, Enter, Space functionality

✅ Dynamic on-screen layout with highlighted key hover

✅ Touchless typing with Notepad integration

✅ Mathematical operator support (+, -, *, /, %, etc.)

⚠️ Challenges Faced
Minimizing false key detection due to hand instability or camera delay

Ensuring accuracy in different lighting conditions and backgrounds

Mapping fingertip coordinates to dynamic key positions

Maintaining real-time performance while rendering and tracking simultaneously

🚀 Future Improvements
Add support for multi-hand tracking

Incorporate gesture-based click detection (e.g., pinch gesture)

Add voice output for typed letters

Enable dynamic resizing of the keyboard for screen adaptability

Package the application with a GUI installer


