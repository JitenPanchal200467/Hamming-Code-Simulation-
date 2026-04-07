# Hamming Code — AR/VR Experience

An interactive 3D holographic simulation designed to teach and demonstrate the **Hamming(7,4)** error detection and correction algorithm. This project combines modern web technologies with a futuristic "AR/VR" aesthetic to make binary data encoding more engaging.

![Hamming Code Preview](https://via.placeholder.com/800x400/010a12/00f5ff?text=HAMMING+CODE+3D+HUD)

## 🚀 Features

- **Interactive 3D Hologram**: A live 3D render of the 7-bit codeword using **Three.js**.
- **Raycasting Interaction**: Direct manipulation of bits by clicking the floating 3D cubes.
- **Holographic HUD**: Immersive "Heads-Up Display" with real-time status readouts and diagnostic data.
- **Error Injection & Correction**: 
    - Inject random single-bit errors. 
    - Watch the "Glitch" jitter effect on corrupted bits.
    - Run the detector to pinpoint and auto-correct errors with a "Stabilization Pulse."
- **Educational HUD**: Side panels explaining Parity Groups, the bit-position map, and the redundancy formula ($2^r \ge m + r + 1$).

## 🛠️ Technologies

- **Core**: HTML5, Vanilla JavaScript.
- **Graphics**: [Three.js](https://threejs.org/) (WebGL) for the 3D engine.
- **Styling**: Vanilla CSS3 with Glassmorphism, Neon Glows, and CSS Animations.
- **Typography**: Google Fonts (Orbitron, Share Tech Mono).

## 🎮 How to Use

1.  **Clone/Download** this repository.
2.  Open `hamming-code-arvr.html` in any modern web browser (Chrome, Firefox, Edge, or Safari).
3.  **Encode**: Enter 4 data bits and click the "ENCODE" button.
4.  **Interact**: Click the 3D cubes directly to manually flip bits, or use the "INJECT ERROR" button.
5.  **Fix**: Click "DETECT & CORRECT" to see the Hamming algorithm in action.

## 📖 Algorithm Overview

Hamming(7,4) adds 3 parity bits to 4 data bits to create a 7-bit codeword. 
- **Parity Bits (P1, P2, P4)**: Placed at positions that are powers of 2 (1, 2, 4).
- **Data Bits (D1-D4)**: Placed at the remaining positions (3, 5, 6, 7).
- **Syndrome**: Calculated by re-checking parity groups. If the syndrome is non-zero, it directly identifies the bit position of the error.

---
*Created for educational purposes to visualize reliable data transmission.*
