# Digial Oil Lamp 

## Overview
An interactive web-based celebration experience where users light up virtual oil lamps. The project was inspired by traditional festival celebrations and features dynamic lamp lighting with beautiful visual effects.

## ✨ Features
## 🪔 Dynamic Lamp System
Customizable Count: Set the number of lamps via URL parameter (?lamps=12) with a default of 7 lamps

Responsive Layout: Automatically adjusts to screen size (4 lamps/row on desktop, 3 on tablet, 2 on mobile)

Interactive Lamps: Click to toggle lamps on/off (between static and animated GIF states)

Celebration Trigger: When all lamps are lit, a special celebration message appears

## 🎨 Visual Effects
Floating Background Animation: Animated circles floating in the background with random sizes, speeds, and colors

Smooth Transitions: Hover effects and smooth animations for lamps

Responsive Design: Works perfectly on all screen sizes from mobile to desktop

## 🎵 Background Music
Auto-playing Music: Background music starts automatically (with user interaction where required)

Keyboard Control: Press M key to toggle music on/off

Visual Audio Indicator: Shows current music status in the top-right corner

Looping Playback: Music continuously loops for uninterrupted experience

## 🚀 How to Use
Basic Usage
Open index.html in a web browser

Click on any lamp to light it up (toggles between on/off states)

Light all lamps to trigger the celebration message

Advanced Features
Custom Lamp Count: Add ?lamps=N to URL (e.g., index.html?lamps=15)

Music Control: Press M key anytime to toggle background music

Screen Adaptation: Resize browser to see automatic layout adjustment

## 🛠️ Setup Instructions
### 1. Required Files
```aiignore


project-folder/
│
├── index.html
├── style.css          (if using separate CSS)
├── animation.css      (if using separate CSS)
│
├── lamp.png           (lamp off state)
├── t-lamp.gif           (lamp on state - animated)
├── lamptr.png         (hidden lamp image)
├── background.jpg            (background image)
│
└── music.mp3 (optional background music)
```

## 2. Adding Background Music
Place your music file in the project folder

Supported formats: MP3

Update the audio source in the HTML:

```html
<source src="music.mp3" type="audio/mpeg">
```
## 3. Customization
Change default lamp count: Modify the default value in the JavaScript (currently 7)

Adjust colors: Edit CSS variables 

Modify animation: Change circle animation parameters in the JavaScript

## Browser Compatibility
Chrome (recommended)

Firefox

Safari

Edge

Note: Some browsers may require user interaction before playing audio

👨‍💻 Development
File Structure
```aiignore


├── HTML Structure
│   ├── Background image container
│   ├── Audio controls panel
│   ├── Celebration message
│   ├── Hidden lamps section
│   ├── Dynamic lamps container
│   └── Background animation container
│
├── CSS Components
│   ├── Responsive lamp grid
│   ├── Floating animation effects
│   ├── Celebration animations
│   ├── Audio control styling
│   └── Interactive hover states
│
└── JavaScript Functionality
    ├── Dynamic lamp generation
    ├── Lamp state management
    ├── Responsive layout calculation
    ├── Background animation generation
    ├── Celebration detection
    └── Audio control system
```

### Key Functions
generateLamps(): Creates lamp grid based on screen size

toggleLamp(index): Handles lamp state changes

generateCircles(): Creates background animations

toggleAudio(): Controls music playback

showCelebration(): Displays celebration message

## 🙏 Credits & Acknowledgements
Major Credit to Original Project:
This project is heavily inspired by and uses resources from Diluk Chamika's Yadham Swara 2023 Oil Lamp Project. Many visual assets, CSS styles, and the core concept were adapted from this original work.

Original Assets Used:
Lamp images (lamp.png, lamp.gif, lamptr.png)

CSS styling and animation concepts

Layout and design inspiration

Interactive lamp functionality concept

Additional Features Added:
Dynamic lamp count via URL parameters

Responsive layout adaptation

Background music system with keyboard controls

Enhanced visual animations

Celebration message system

Improved user interface