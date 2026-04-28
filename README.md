# TriageAI 🏥

> **AI-Powered Mass Casualty Triage System** — Built for Google Solution Challenge 2026

TriageAI is an intelligent emergency triage system that leverages **Google Gemini's multimodal AI** to help first responders classify patients, optimize resource allocation, and coordinate hospital routing during mass casualty events.

## 🎯 Problem Statement

During mass casualty events (train crashes, building collapses, stampedes), emergency rooms are overwhelmed. Triage decisions are made under extreme stress, leading to suboptimal resource allocation and preventable deaths. India faces approximately 450+ mass casualty events annually.

## 💡 Solution

TriageAI provides:

- **🗣️ Voice-First Triage** — Paramedics describe injuries verbally; Gemini transcribes and auto-classifies severity (Red/Yellow/Green/Black)
- **📸 Photo Assessment** — Snap a photo of injuries; Gemini Vision provides preliminary assessment
- **📊 Real-Time Dashboard** — Hospital administrators see patient flow, resource utilization, and predicted surge
- **🏥 Smart Hospital Routing** — AI-optimized patient-to-hospital routing based on severity, specialty needs, and distance
- **📦 Resource Management** — Track ambulances, beds, surgeons, blood supply in real-time

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **Gemini API** | Multimodal AI (text, vision, voice analysis) |
| **Firebase** | Authentication, Firestore, Cloud Hosting |
| **Google Maps Platform** | Hospital routing & geolocation |
| **React + Vite** | Frontend framework |
| **Google Cloud** | Infrastructure (via Firebase) |

## 🎯 UN Sustainable Development Goals

- **SDG 3** — Good Health & Well-Being
- **SDG 11** — Sustainable Cities & Communities

## 🏗️ Architecture

```
┌─────────────────────────────────────────────┐
│                  Frontend                    │
│          React + Vite (Firebase Hosting)     │
├─────────────────────────────────────────────┤
│                                              │
│  ┌──────────┐  ┌───────────┐  ┌──────────┐ │
│  │  Voice   │  │   Photo   │  │   Text   │ │
│  │  Input   │  │   Input   │  │  Input   │ │
│  └────┬─────┘  └─────┬─────┘  └────┬─────┘ │
│       │              │              │        │
│       └──────────────┼──────────────┘        │
│                      ▼                       │
│            ┌─────────────────┐               │
│            │   Gemini API    │               │
│            │  (Multimodal)   │               │
│            └────────┬────────┘               │
│                     ▼                        │
│     ┌───────────────────────────┐            │
│     │   Triage Classification   │            │
│     │  Severity: RED/YELLOW/    │            │
│     │  GREEN/BLACK              │            │
│     └───────────┬───────────────┘            │
│                 ▼                            │
│  ┌──────────────────────────────────┐        │
│  │  Firebase Firestore (Real-time)  │        │
│  │  - Patient Records              │        │
│  │  - Resource Tracking            │        │
│  │  - Hospital Status              │        │
│  └──────────────┬───────────────────┘        │
│                 ▼                            │
│     ┌─────────────────────┐                  │
│     │ Google Maps Platform│                  │
│     │ Hospital Routing    │                  │
│     └─────────────────────┘                  │
└─────────────────────────────────────────────┘
```

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/triage-ai.git

# Install dependencies
cd triage-ai
npm install

# Set up environment variables
cp .env.example .env
# Add your Gemini API key to .env

# Start development server
npm run dev
```

## 📸 Screenshots

[Screenshots will be added]

## 🎬 Demo Video

[3-minute demo video link]

## 👥 Team

- **Team Name:** [Your Team Name]
- **Team Leader:** [Your Name]

## 📄 License

MIT License

---

Built with ❤️ for **Google Solution Challenge 2026** | Powered by **Google Gemini**
