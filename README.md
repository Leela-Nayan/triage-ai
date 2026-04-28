# TriageAI 

> **AI-Powered Mass Casualty Triage System** — Built for Google Solution Challenge 2026

TriageAI is an intelligent emergency triage system that leverages **Google Gemini's multimodal AI** to help first responders classify patients, optimize resource allocation, and coordinate hospital routing during mass casualty events.

## Problem Statement

During mass casualty events (train crashes, building collapses, stampedes), emergency rooms are overwhelmed. Triage decisions are made under extreme stress, leading to suboptimal resource allocation and preventable deaths. India faces approximately 450+ mass casualty events annually.

## Solution

TriageAI provides:

- **Voice-First Triage** — Paramedics describe injuries verbally; Gemini transcribes and auto-classifies severity (Red/Yellow/Green/Black)
- **Photo Assessment** — Snap a photo of injuries; Gemini Vision provides preliminary assessment
- **Real-Time Dashboard** — Hospital administrators see patient flow, resource utilization, and predicted surge
- **Smart Hospital Routing** — AI-optimized patient-to-hospital routing based on severity, specialty needs, and distance
- **Resource Management** — Track ambulances, beds, surgeons, blood supply in real-time

## Tech Stack

| Technology | Purpose |
|---|---|
| **Gemini API** | Multimodal AI (text, vision, voice analysis) |
| **Firebase** | Authentication, Firestore, Cloud Hosting |
| **Google Maps Platform** | Hospital routing & geolocation |
| **React + Vite** | Frontend framework |
| **Google Cloud** | Infrastructure (via Firebase) |

## UN Sustainable Development Goals

- **SDG 3** — Good Health & Well-Being
- **SDG 11** — Sustainable Cities & Communities

## Architecture

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



## Screenshots

<img width="2940" height="1496" alt="Screenshot 2026-04-28 at 23 05 24" src="https://github.com/user-attachments/assets/f22b568b-1172-46b0-a4f2-57124e8f66cb" />
<img width="2940" height="1496" alt="Screenshot 2026-04-28 at 23 08 33" src="https://github.com/user-attachments/assets/e1c84e8c-bcb9-4b62-80d7-17898d3b17a5" />
<img width="2940" height="1490" alt="Screenshot 2026-04-28 at 23 09 15" src="https://github.com/user-attachments/assets/7d57e0f4-bae0-490e-a249-5f4a4b1e7b13" />
<img width="2940" height="1486" alt="Screenshot 2026-04-28 at 23 09 21" src="https://github.com/user-attachments/assets/33204f3b-5dcf-4c91-8d10-32c8379b6721" />
<img width="2940" height="1498" alt="Screenshot 2026-04-28 at 23 09 29" src="https://github.com/user-attachments/assets/b948bdc9-c2e8-4a96-acfa-f6a211c53a31" />
<img width="2940" height="1496" alt="Screenshot 2026-04-28 at 23 09 40" src="https://github.com/user-attachments/assets/7b2cdbf5-3a7a-416f-8d4e-b22bad10dad1" />
<img width="2938" height="1514" alt="Screenshot 2026-04-28 at 23 09 48" src="https://github.com/user-attachments/assets/b66c7826-25e2-4399-bf4e-3b8125a62af6" />
<img width="2940" height="1524" alt="Screenshot 2026-04-28 at 23 10 06" src="https://github.com/user-attachments/assets/803abfe6-11ae-4874-af49-484ce7c6432d" />


## Demo Video



## Team

- **Team Name:** Overwatch
- **Team Leader:** Leela Nayan K.P
- Rushikesh Yadav Vadlakonda
- Y. Rithwik

