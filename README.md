# 🟣 Auralis

A sleek, modern face recognition attendance app that runs entirely in your browser. Auralis detects and recognises students through a live camera or a class photo, marks attendance in seconds, and turns the results into records, insights, and shareable reports. It has a live dashboard and multi-language support.

---

## ✨ Features

- 🎯 **Face recognition attendance** — detect and identify students from a live camera feed or an uploaded class photo
- 📸 **Group photo scanning** — tiled, multi-pass detection finds many faces in a single classroom photo
- 👁️ **Blink liveness check** — students must blink to be verified, which blocks photo-based spoofing
- 🔊 **Voice greeting** — the app speaks a welcome to each student in the selected language
- 🔔 **Check-in chime** — a short sound confirms every successful mark (can be turned off)
- 🔄 **Flip camera** — switch between front and rear cameras on phones and tablets
- 🖥️ **Three scan modes** — Classroom, Kiosk (gate, with a big welcome banner), and Strict (exam, stricter matching plus mandatory blink)
- ⏰ **Late tracking** — set a start time and grace period, and late arrivals are flagged automatically
- 📋 **Yet-to-arrive list** — see who hasn't been marked yet, live, during a scan
- 🏫 **Grade and division classes** — organise students by Grade 1–12 and Division A–F, and filter every view by class
- 👩‍🎓 **Student enrolment** — add one or many photos, edit names and roll numbers, assign a class, and add extra photos to improve accuracy
- 🌗 **Dark and light mode** — one-tap theme toggle that follows your system theme by default and remembers your choice
- 📊 **Live dashboard** — animated attendance ring, present / late / absent counts, a 7-day trend, and recent check-ins on the home screen
- 📈 **Insights** — per-student attendance bars, at-risk students (below 75%), a 14-day heatmap, top attendance, and most often late
- 🗂️ **Records** — view any date or class, search by name or roll number, filter by status, and correct entries by hand
- ✅ **Mark all present** — one click to fill a whole class, then untick the exceptions
- 📤 **Export and share** — download a daily CSV or a full attendance report, copy a summary, or send it on WhatsApp
- 🖨️ **Print-ready records** — print the attendance table straight from the browser
- 🌍 **Multi-language interface** — English, हिन्दी, ಕನ್ನಡ, and Español
- 🎛️ **Detection tuning** — adjust detection sensitivity and match strictness to suit your lighting and camera
- 💾 **Backup and restore** — export all students and attendance to a JSON file and load it back on any device
- 📱 **Responsive design** — works on desktop, tablet, and mobile screens
- 🖼️ **Kiosk fullscreen** — go fullscreen for a wall-mounted or gate-side setup

---

## 🔒 Privacy

- 🏠 **Runs locally** — all recognition happens in your browser; no images or student data are sent to a server
- 💽 **Local storage only** — students, face data, attendance, and preferences are saved on the device you use
- 🧹 **You stay in control** — clear today's records or delete all data at any time from Settings

---

## 🚀 Getting Started

1. **Open the app** — open `auralis.html` in a modern browser (Chrome, Edge, or Safari).
2. **Enrol students** — go to **Students**, add clear front-facing photos, fill in names, roll numbers, and class, then press **Save students**.
3. **Set up the session** — in **Scan**, choose the grade and division, the mode, and an optional start time with grace minutes.
4. **Start scanning** — press **Start camera** or upload a **Class photo**. Recognised students are marked automatically.
5. **Review and share** — check **Insights** and **Records**, then export a CSV or share the summary.

> 💡 The camera needs a secure context. Open the file through `localhost` or `https`, or use the class photo upload option.

---

## 🧰 Tech Stack

- 🌐 **HTML, CSS, and vanilla JavaScript** — a single self-contained file, no build step
- 🧠 **face-api.js (`@vladmandic/face-api`)** — face detection, landmarks, expressions, and recognition
- 🎨 **CSS variables** — powers the dark and light themes
- 🗣️ **Web Speech API** — voice greetings
- 🔉 **Web Audio API** — check-in chime
- 💾 **localStorage** — on-device data and preferences

---

## ⚙️ Settings

| Setting | What it does |
| --- | --- |
| 🔍 Detection sensitivity | Lower values detect more (and smaller) faces |
| 🎚️ Match strictness | Controls how closely a face must match an enrolled student |
| 💾 Backup / Restore | Save or load all data as a JSON file |
| 🗑️ Clear today / Delete all | Reset today's attendance or wipe everything |

---

## 📁 Project Structure

```
auralis/
├── auralis.html   # the entire app (UI, styles, and logic)
└── README.md
```

---

## ⚠️ Notes

- 🌐 An internet connection is needed on first load to fetch the face-api library and models from a CDN.
- 💡 Good lighting and clear, front-facing enrolment photos give the best accuracy.
- 🧪 Face recognition can make mistakes, so use **Records** to review and correct attendance when it matters.
- 🔐 Browser storage is per device and per browser. Use **Backup data** before clearing your browser data or switching devices.

---

## 📜 License

Add your preferred license here (for example, MIT).
