# MonReader
# PROJECT X697MdyV9MDIqiKx
# 📚 MonReader: Intelligent Page-Flip Detection & OCR for Document Digitization

MonReader is a mobile-first document digitization solution built for the blind, researchers, and anyone needing **fully automatic**, **high-speed**, and **high-quality** bulk document scanning.

This repository contains the core module for **page-flip detection using deep learning**, integrated with a robust **OCR pipeline**, deployed as a web application.

---

## 🚀 Features

- 📄 **Page-Flip Detection** from smartphone videos using single image classification
- 🔎 **Optical Character Recognition (OCR)** with advanced deep learning models
- 🧠 **Machine Learning Models**: Custom CNN, ResNet, EfficientNet, SqueezeNet
- 🌐 **Web App**: Built with Flask, containerized with Docker, and deployed on AWS

---

## 🧠 Problem Statement

Develop a model that can detect whether a page is being flipped using a **single image**, extracted from smartphone video recordings. This is used to automatically trigger document scanning without manual input.

---

## 📁 Dataset Overview

- Videos captured on smartphones
- Split into short clips, labeled as `flip` or `not flip`
- Frames extracted and saved with format: `VideoID_FrameNumber`

### Data Split

- **Training**: 1228 `not flip`, 1162 `flip`
- **Testing**: 285 `not flip`, 306 `flip`

---

## 🧪 Model Performance (F1 Score)

| Model         | F1 Score |
|---------------|----------|
| Custom CNN    | 81%      |
| ResNet        | 68%      |
| EfficientNet  | 85%      |
| **SqueezeNet**| **100%** ✅ |

SqueezeNet provided top performance with compact architecture, making it suitable for real-time mobile inference.

---

## 🔤 OCR Integration

Tested multiple state-of-the-art OCR models:

- `Pytesseract`
- `Idefics`
- `LLaVA`
- `Shikra`
- `Gemma`
- `Donut`
- **Hybrid:** Idefics + Sesame

---

## 🌍 Deployment

The entire pipeline was deployed using:

- ✅ **Flask Web Framework**
- ✅ **Docker** for containerization
- ✅ **AWS** for cloud hosting

Users can upload documents and receive high-quality, OCR-processed text automatically.

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/monreader.git
cd monreader

## 📫 Contact

**Project Maintainer:** \[Ernest Braimoh]

📧 Medium: [Ernest Braimoh]_(https://medium.com/@akindream/building-monreader-smart-page-flip-detection-meets-powerful-ocr-0b7fe62886a0)

🔗 LinkedIn: [Ernest Braimoh]_(https://www.linkedin.com/posts/ernest-braimoh_ai-computervision-machinelearning-activity-7357017049199460352-bmih?utm_source=share&utm_medium=member_desktop&rcm=ACoAACJ5f84BSF16YQBlNnzy86sMhIc99PdU8l0)

🔗 Youtube: [Ernest Braimoh]_()
