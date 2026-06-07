# 👽 Ben 10: Omnitrix AR Experience

![Omnitrix AR Banner](assets/omnitrix/New_OS_Omnitrix_artwork.webp)

A fully interactive, web-based Augmented Reality (AR) experience that brings the iconic Ben 10 Omnitrix to life directly in your browser. No apps, no downloads—just step in front of your webcam, and the Omnitrix will physically lock onto your wrist. 

This project uses advanced AI hand-tracking to let you physically interact with the watch using real-life gestures from the show!

## ✨ Features

- **🦾 True AR Tracking:** Uses AI to perfectly map a 3D model of the Original Series (OS) Omnitrix onto your left wrist in real-time.
- **✋ Physical Gesture Controls:** 
  - **Activate:** Flick your left wrist upwards.
  - **Dial Selection:** Use your right thumb and index finger to physically grab and twist the 3D dial to cycle through 10 different aliens.
  - **Transform:** Slam your right hand down onto the watch face!
- **💥 Immersive Transformations:** Hitting the watch triggers screen-shake, particle bursts, and full-screen visual effects leading instantly into the official transformation sequences.
- **📱 Cross-Platform:** Works entirely in the browser on desktop and mobile (Requires Safari/Chrome—in-app browsers like Instagram's built-in browser are not supported due to camera security restrictions).

## 🛠️ Technology Stack

- **HTML5 / CSS3 / Vanilla JavaScript**
- **[Three.js](https://threejs.org/):** Used to render, light, and perfectly scale the 3D `.glb` Omnitrix model into the real-world environment.
- **[Google MediaPipe](https://developers.google.com/mediapipe):** State-of-the-art AI vision processing used to track 42 distinct hand landmarks in real-time at 60fps.
- **Custom Physics Engine:** Includes advanced exponential smoothing, velocity tracking, and predictive impact detection so the watch feels heavy and attached to your physical body.

## 🚀 How to Run Locally

1. Clone this repository to your local machine.
2. Because the app uses the webcam and fetches 3D/Video assets, it **must** be run through a local web server (opening the `.html` file directly will trigger CORS security blocks).
3. Open your terminal in the project folder and run:
   ```bash
   python -m http.server 8000
   ```
   *(Or use any local server like VSCode Live Server or `npx serve`)*
4. Open your browser and navigate to `http://localhost:8000`

## 📲 How to Play

1. Allow camera permissions when prompted.
2. Stand back so the camera can clearly see your upper body and hands.
3. Bring your **left arm** up. The watch will appear.
4. Bring your **right hand** close and use your thumb and index finger to physically "pinch and twist" the green dial.
5. Once you've selected your alien, **SLAM** your right hand down onto the watch to transform!

## ⚠️ Note on Mobile/Instagram

If you are visiting this project from a link on Instagram, **you must open it in an external browser** (Safari or Chrome). Instagram's built-in browser prevents websites from accessing the camera, which will stop the AR from working.

---
*Disclaimer: This is a fan-made project. All Ben 10 characters, designs, and video assets belong to Cartoon Network and Warner Bros. Discovery.*
