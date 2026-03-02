# Monitoring-System
Smart Mobile Monitoring System
A lightweight, web-based utility designed to help users manage screen time through real-time tracking, threshold alerts, and usage reporting. This tool simulates a mobile monitoring environment using JavaScript and the Web Audio API.

🚀 Features
Customizable Time Limits: Set your maximum allowed usage in minutes.

Real-time Tracking: Live "Elapsed Time" display showing usage down to the second.

Tiered Alert System:

75% Warning: Soft alert when you approach your limit.

90% Warning: Critical alert to wrap up your tasks.

100% Limit: Final notification and simulated system shutdown.

Multi-Sensory Feedback: Includes JavaScript-driven sound (sine wave oscillator) and device vibration (for supported mobile browsers).

Usage Reports: Quick summary of total minutes consumed during the session.

Reset Functionality: Easily clear current progress and start a new monitoring cycle.

🛠️ Technical Overview
The system is built as a single-page application (SPA) using standard web technologies:

HTML5: Structured interface with semantic inputs.

CSS3: Clean, responsive UI with a focused "Container" layout.

JavaScript (Vanilla): * setInterval() for precise time tracking.

Web Audio API: Generates a synthetic "beep" without requiring external mp3 files.

Vibration API: Triggers haptic feedback on compatible hardware.

📖 How to Use
Open the File: Open index.html in any modern web browser (Chrome, Firefox, or Safari).

Set Limit: Enter the number of minutes you wish to stay active in the input field.

Start: Click Start Monitoring.

Monitor: Keep the tab open. The system will alert you as you hit usage milestones.

Review: Click Generate Reports at any time to see your exact usage in decimal minutes.

⚠️ Limitations & Notes
[!IMPORTANT]
Simulated Environment: As this is a web-based tool, the "System Shutdown" feature is a simulation. Standard web browsers do not have the permissions to shut down a physical device or close other applications for security reasons.

Audio/Vibration: Some browsers require a "User Gesture" (like clicking the Start button) before sound or vibration can be triggered.

Background Throttling: If the tab is minimized, some browsers may throttle the setInterval frequency to save power, which might slightly affect timer accuracy.

🔧 Future Enhancements
[ ] LocalStorage integration to save usage history across sessions.

[ ] Dark Mode support for nighttime monitoring.

[ ] Graphical charts for usage trends using Chart.js.