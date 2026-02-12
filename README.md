# 📍 GeoLink – Real-Time Location Sharing System

GeoLink is a real-time, consent-based live location tracking web application built using:

- 🌐 HTML, CSS, JavaScript  
- 🔥 Firebase Realtime Database  
- 🗺️ Leaflet (OpenStreetMap)  
- 🚀 GitHub Pages  

It allows a **Sender** to share live GPS location and an **Admin Dashboard** to track that location instantly in real time.

---

## 🚀 Live Demo

Sender:
https://satyam-50.github.io/location/

Admin Dashboard:
https://satyam-50.github.io/location/admin.html

---

## ⚙️ How It Works

1. Sender clicks **Start Live Sharing**
2. Browser fetches GPS coordinates using Geolocation API
3. Coordinates are pushed to Firebase at:

   locations/target_user

4. Admin dashboard listens to that path
5. Map updates automatically without refresh

---

## 🛠️ Tech Stack

- HTML, CSS (Dark UI Design)
- Vanilla JavaScript
- Firebase Realtime Database
- Leaflet.js for map rendering
- GitHub Pages for deployment

---

## 🔥 Firebase Setup

### 1️⃣ Create Firebase Project
Go to:
https://console.firebase.google.com/

Create a new project.

---

### 2️⃣ Enable Realtime Database

- Go to **Build → Realtime Database**
- Click **Create Database**
- Choose location
- Start in Test Mode

---

### 3️⃣ Set Database Rules

Go to **Rules tab** and paste:

```json
{
  "rules": {
    ".read": true,
    ".write": true
  }
}
