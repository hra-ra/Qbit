# 📚 Bunkr

A lightweight, zero-dependency **Progressive Web App (PWA)** engineered with Vanilla JavaScript, HTML5, and CSS3 that lets students calculate safe-to-skip thresholds, log attendance, and manage academic schedules offline.

---

## ⚡ Live App

You can launch the web app instantly on any device here: https://bunkr-sepia.vercel.app/# 👈 

---

## 🎯 Overview

Bunkr eliminates the math behind tracking college attendance. Powered by an offline-first architecture, the application computes precise attendance safety margins, tracks class sessions, handles holiday exceptions, and lets you import schedules without hitting a backend server. Everything runs directly in the client browser using modern Web APIs for high performance and total data privacy.

### Core Highlights:

* **Zero Dependencies:** Built purely on standard browser APIs (`Web Storage`, `Web Audio`, `History API`) without heavy external frameworks.
* **Installable & Offline-First:** Fully functional without an active internet connection via a dedicated `Service Worker` and web app manifest.
* **Smart Attendance Logic:** Instant algorithms for calculating margin-for-error and safe bums per subject.
* **Native PWA Integration:** Seamless home-screen installation and native-like responsiveness across desktop and mobile.

---

## 📂 Architecture

```text
├── index.html          # Core layout & HTML5 structure
├── manifest.json       # PWA metadata & web app configuration
├── service-worker.js   # Offline caching logic & asset management
├── css/
│   └── style.css       # Custom styles & responsive layout
└── js/
    ├── scan.js          # Application bootstrapper & event listeners
    ├── state.js        # LocalStorage state management
    ├── render.js       # Dynamic UI rendering logic
    ├── stats.js        # Attendance calculation algorithms
    └── calendar.js     # Timetable & holiday handling module