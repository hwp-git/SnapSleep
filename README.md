# 🌙 Snap Sleep: Self-Evolving Multi-Modal AI Sleep Agent

[![Agent-Native](https://img.shields.io/badge/Architecture-Agent--Native-red.svg)](#)
[![Multi-Modal AI](https://img.shields.io/badge/AI-Multi--Modal-purple.svg)](#)
[![Edge to Cloud](https://img.shields.io/badge/Scale-Edge_to_Cloud-blue.svg)](#)
[![iOS](https://img.shields.io/badge/iOS-Native%20Vision-blue.svg)](https://developer.apple.com/ios/)

> **Snap Sleep** is an agent-native, privacy-first, and self-evolving sleep health ecosystem. We are transforming multi-modal AI (vision and acoustics) into sensory infrastructure. Our AI agent doesn't just "diagnose" the mechanical causes of snoring—it actively "intervenes" by prescribing a customized hardware solution (our proprietary X-Wing module) and continuously self-optimizes its models based on real-world efficacy, creating an ever-improving Physical-Digital Recovery Loop.

<img width="1408" height="768" alt="Lifestyle_snoring_overlay1" src="https://github.com/user-attachments/assets/fab37601-f35f-4911-be2e-50ec3fe1fd21" />

---

## 🚀 The Vision: Sleep Infrastructure in the Agent-Native Era
Traditional sleep apps are passive dashboards. Snap Sleep is an **Autonomous Health Agent**.
1. **Sense (Multi-Modal Infrastructure):** Utilizes edge computing (initially via iPhone, scaling to dedicated night vision cameras) to capture facial biomechanics and airflow acoustics in low-light environments.
2. **Diagnose:** The AI engine accurately identifies the physical root causes of snoring (jaw drop, tongue collapse, palatal flutter).
3. **Intervene:** The agent prescribes a specific physical intervention—our proprietary, rapid-3D-printable `X-Wing` silicone matrix.
4. **Evolve:** By measuring overnight biometric changes and subjective user feedback, the AI agent continuously trains and self-improves its diagnostic and treatment models.

---

## 🛡️ Privacy-First & Scalable
During the POC phase, we strictly adhere to a **"Zero Cloud Video Uploads"** policy.
All visual data extraction is processed in real-time on the **local device (Edge AI)** via Apple's built-in Neural Engine. As we scale, we only push de-identified numerical tags (e.g., timestamps, angle offsets, decibel parameters) to the cloud for deep model training. This ensures the highest privacy standards while empowering the AI to self-evolve.

---

## 🏗️ Core System Architecture

### 1. Multi-Modal Sensory Engine
* **Visual Feature Engine (Vision Framework):** Utilizes `VNDetectFaceLandmarksRequest` to track facial dynamics in low light. Real-time calculation of the Y-axis distance between the Upper and Lower Lip accurately captures "Jaw Drop" events.
* **Acoustic Feature Engine (AVFoundation):** Uses `AVAudioRecorder` (`isMeteringEnabled = true`) to monitor the frequency and decibels (dB) of obstructed airflow, perfectly syncing with the visual timeline.

### 2. Diagnostic Brain & Self-Learning Loop
Converts the captured data into a structured `5W (What, When, Why, Where, Who)` medical log and cross-references it:

| Medical/Anatomical Root Cause (The "Why") | Multi-Modal AI Logic (Vision + Sound) | AI Prescribed Intervention (The Hardware) |
| :--- | :--- | :--- |
| **Mouth Wheezing** | `Extreme Jaw Drop Angle` + `Continuous dry airflow sound` | **X-Wing Silicone Wings** (Physically restricts oral turbulence) |
| **Tongue Base Collapse** | `Lips closed or slightly parted` + `Sudden blockages / Choking` | **X-Wing Internal Suction Bulb** (Stabilizes and gently pulls tongue) |
| **Palatal Snoring** | `Jaw slightly closed` + `Continuous low-frequency rumble (High dB)` | **X-Wing Basic Kit** (Alters oral cavity tension) |
| **Nasal Snoring** | `Jaw Drop = 0 (Lips tightly closed)` + `High-frequency muffled hum` | **Nasal Dilator Strip** |

---

## 🗺️ Roadmap

This is a revolution scaling from edge computing to a full hardware-enabled ecosystem:

* [x] **Phase 1 (Current) - Edge AI & MVP:** Local multi-modal Proof-of-Concept based on iOS Vision & Audio Frameworks, paired with the Bambu Lab A1 rapid-prototyped X-Wing physical device.
* [ ] **Phase 2 (Scaling) - Cloud Computing & Self-Evolving:** Cloud integration for deep pattern analysis. Implementing User Feedback Loops to allow the AI agent to auto-train and optimize its recommendation models based on real overnight efficacy.
* [ ] **Phase 3 (Ecosystem) - IoT & Night Vision:** Launching the proprietary "Snap Sleep Night Vision Camera" with embedded machine vision and smart sleep peripherals, completing the self-improvement ecosystem for premium users.

---

## 🔒 Open Source & IP Statement
This repository acts as a **Showcase**, designed to demonstrate the team's Agent-Native architectural capabilities and technical vision to investors and partners. 
To protect Snap Sleep's multi-modal core algorithms, self-evolving weights, and the physical parameters of the X-Wing, our core business logic is maintained as closed-source. We will gradually decouple and open-source our UI components, visualization funnels, and basic APIs to give back to the developer community.

*Designed with 🌙 by the Snap Sleep Team. (Silicon Valley Software DNA x Taiwan Hardware Iteration)*
