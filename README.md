# Spinning CAD 🚴‍♂️💨

A lightweight, minimalist, and ad-free web application designed specifically for **indoor cycling / spinning**. Its purpose is to connect directly with a Bluetooth Low Energy (BLE) cadence sensor using the browser's native Web Bluetooth API to display **real-time RPM**, a color-coded zone indicator, and an integrated countdown timer.

Tailored for short 10 or 15-minute post-meal training blocks, with no accounts, no trackers, and no bloatware.

---

## 🚀 Key Features

* **Direct Bluetooth Connection (Web Bluetooth):** Instantly pairs with any standard Bluetooth cadence sensor (Wahoo, Magene, Garmin, Moofit, etc.).
* **Giant RPM Display:** Large numbers optimized for quick glancing while riding.
* **Color-Coded Zone Indicator (Traffic Light):** 
  * 🔵 **Below 75 RPM:** Low cadence / Paused.
  * 🟡 **75 - 79 RPM:** Approaching optimal zone.
  * 🟢 **80 - 90 RPM:** **Optimal Zone** (ideal for post-meal metabolic activation).
  * 🟠 **Above 92 RPM:** High pace.
* **Smart Auto-Start:** The 10 or 15-minute countdown timer starts automatically as soon as cadence reaches $\ge 40\text{ RPM}$.
* **Session Statistics:** Computes average RPM and total pedal revolutions upon completion.
* **Anti-Sleep (WakeLock):** Keeps the phone screen awake throughout the entire workout.

---

## 📱 Requirements

Because it uses the **Web Bluetooth** API, the app requires:
1. **A compatible browser:** Google Chrome or Microsoft Edge on Android / PC / Mac (Chromium-based browsers support Web Bluetooth). *Note: On iOS devices (iPhone/iPad), browsers use WebKit and do not natively support Web Bluetooth.*
2. **A Bluetooth cadence sensor** (Standard *Cycling Speed and Cadence* - CSC profile with UUID `0x1816`).
3. **HTTPS connection** (or `localhost`) for browser Bluetooth permissions.

---

## 🛠️ How to Use / Install on Your Phone

1. Open the project URL in **Google Chrome for Android**.
2. Tap the three vertical dots menu (`⋮`) in the top-right corner of the browser.
3. Select **"Add to Home Screen"** or **"Install app"**.
4. Done! A shortcut will be created on your home screen acting like a native app.

---

## ⚙️ Quick Start

1. Give the crank a couple of turns to wake up your cadence sensor.
2. Open the app on your phone and tap the **"Connect CAD"** button in the top left.
3. Select your device from the browser popup window.
4. Once connected, the status dot will turn **green**, choose your preset time (10m or 15m), and start pedaling.

---

## 📄 License

This project is open-source under the [MIT](LICENSE) license. Feel free to adapt or improve it for your personal workouts.
