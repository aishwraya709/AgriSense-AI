# 🌾 AgriSense‑AI  
### *Integrating Soil Microbiome Intelligence with AI‑Driven Precision Farming*

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![Website](https://img.shields.io/badge/website-live-brightgreen)](https://your-domain.com)

---

## 📌 Overview

**AgriSense‑AI** is an open‑source research platform that fuses **metagenomic soil microbiome profiling** with **real‑time IoT sensor data** and **ensemble machine learning** to generate actionable, site‑specific crop management recommendations. Designed for tropical agroecosystems under Taiwan’s New Southbound Policy, it targets smallholder farmers in Southeast and South Asia.

Our novel approach:
- Characterizes microbial communities (16S rRNA & shotgun metagenomics) and functional gene pathways.
- Integrates IoT soil data (moisture, temperature, pH, EC) via LoRaWAN.
- Trains a Random Forest + XGBoost ensemble on 1,200+ features to predict optimal fertilizer, irrigation, and bio‑input regimes.
- Delivers interpretable recommendations via a **multilingual Progressive Web App** (English, Mandarin, Hindi) with offline support.

This repository contains the **full source code** for the AgriSense‑AI dashboard, the ML pipeline, IoT firmware, and the comparative Taiwan–India field trial framework.

---

## ✨ Key Features

- **Microbiome Intelligence** – 16S rRNA and shotgun metagenomic analysis (QIIME2, PICRUSt2) with biomarker discovery.
- **Live IoT Dashboard** – Real‑time soil sensor streaming (simulated or hardware) with trend charts and health scores.
- **AI Yield Simulator** – Interactive sliders for soil carbon, diversity index, and nitrogen to predict yield and fertilizer savings.
- **SHAP Explainability** – Feature importance visualisation showing *why* a recommendation is made.
- **Twin‑Site Map** – Comparative view of NPUST (Taiwan) and Maharashtra (India) experimental locations.
- **Carbon Sequestration Module** – Estimates additional CO₂‑eq captured per hectare.
- **Offline‑First PWA** – Works in low‑bandwidth environments; syncs data when online.
- **Multilingual UI** – Easily switch between English, Mandarin, and Hindi.
- **Open‑Source Stack** – All software components are free and well‑documented.

---

## 🧬 Research Background

This project was submitted to the **New Southbound Policy Elite Study Program (NSPESP)** at National Pingtung University of Science and Technology (NPUST), Taiwan. It addresses global food security by unlocking the "hidden intelligence" of the soil microbiome, which conventional soil tests ignore.

- **Problem:** 33% of soils degraded, over‑reliance on chemical inputs, lack of biological data in precision ag.
- **Solution:** A low‑cost, transferable AI system that uses microbes as early‑warning indicators and decision guides.
- **Impact:** 15‑25% fertilizer reduction, 10‑20% yield increase, 40‑50% disease reduction.

---

## 🧰 Tech Stack

| Layer               | Technologies                                                                 |
|---------------------|-------------------------------------------------------------------------------|
| **Frontend**        | HTML5, CSS3, JavaScript (Vanilla), Chart.js, Leaflet.js, Font Awesome        |
| **ML & Data**       | Python 3.9+, pandas, numpy, scikit‑learn, XGBoost, QIIME2, PICRUSt2, SHAP    |
| **IoT Firmware**    | C++ (ESP32/Arduino), LoRaWAN, MQTT, InfluxDB (time‑series)                   |
| **Cloud / Backend** | AWS (EC2, S3, RDS), Node.js / Flask (optional), Docker (optional)            |
| **Database**        | PostgreSQL (agronomic data), InfluxDB (sensor logs), NCBI SRA (sequences)    |
| **Deployment**      | GitHub Pages (for static demo), Netlify / Vercel (optional), Docker Compose  |

---

## 🚀 Quick Start (Website Demo)

The interactive website is already built and can be run locally:

```bash
# Clone the repository
git clone https://github.com/aishwraya709/AgriSense-AI.git
cd agrisense-ai
