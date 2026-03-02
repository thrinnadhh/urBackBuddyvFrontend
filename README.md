# UrBackBuddyAI v1.1 - Frontend

UrBackBuddyAI is an intelligent posture-monitoring application that uses computer vision to track your posture in real-time and provide interactive, 3D visual feedback.

## Features
- **Real-Time Posture Tracking**: Utilizes TensorFlow.js (MoveNet) to detect body keypoints and calculate your posture score (Neck, Shoulders, Spine).
- **Interactive 3D Buddy**: A WebGL-powered Robot avatar (React Three Fiber) that reacts to your posture. It floats happily when your posture is good, and slumps/shakes when you need to sit up straight!
- **Sleek UI Dashboard**: A modern, dark-themed dashboard built with React and Tailwind CSS to display your posture score and metrics.
- **Cross-Platform**: Built with Tauri, React, and Vite for cross-platform desktop native performance with web technologies.

## Tech Stack
- **Frontend Framework**: React 19, Vite
- **Styling**: Tailwind CSS v4
- **3D Graphics**: Three.js, `@react-three/fiber`, `@react-three/drei`
- **AI / Computer Vision**: TensorFlow.js, `@tensorflow-models/pose-detection`
- **Native Wrapper**: Tauri

## Getting Started

### Prerequisites
- Node.js
- Rust & Cargo (for Tauri)

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/thrinnadhh/urBackBuddyvFrontend.git
   ```
2. Install dependencies:
   ```bash
   npm install
   ```

### Running Locally
To run the web app in your browser (development mode):
```bash
npm run dev
```

To run the native desktop application (requires Rust):
```bash
npm run tauri dev
```

### Building for Production
```bash
npm run build
```
*(Optionally, use `npm run tauri build` for the desktop release build)*
