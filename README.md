# CrystallineAttachment

> Hybrid NLP + Cybersecurity system for malicious email attachment detection

---

## Overview

CrystallineAttachment is a hybrid cybersecurity project that combines a **RoBERTa-based NLP model** with **static image rendering** to detect and mitigate malicious email attachments.

Traditional antivirus tools rely on signature matching — CrystallineAttachment goes further by analyzing both the **semantic content** of attachments and their **visual rendering behavior**, catching threats that evade conventional filters.

---

## How It Works

```
Email Attachment
      │
      ├──► NLP Analysis (RoBERTa)
      │         └── Classifies text content as malicious / benign
      │
      ├──► Static Image Rendering
      │         └── Captures visual behavior of the attachment
      │
      └──► Combined Decision Engine
                └── Final verdict: Safe / Threat Detected
```

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| NLP Model | RoBERTa (HuggingFace Transformers) |
| ML Pipeline | Scikit-learn, NumPy, Pandas |
| Backend | Python, Flask |
| Rendering | Static image analysis |

---

## Features

- Fine-tuned RoBERTa model for email threat classification
- Static rendering engine to detect visually obfuscated payloads
- Hybrid decision system combining NLP + visual signals
- REST API interface via Flask
- Lightweight and extensible architecture

---

## Project Structure

```
CrystallineAttachment/
├── model/
│   ├── train.py          # RoBERTa fine-tuning
│   └── predict.py        # Inference pipeline
├── rendering/
│   └── static_render.py  # Image rendering module
├── api/
│   └── app.py            # Flask REST API
├── data/
│   └── sample_data/      # Sample email attachments
├── requirements.txt
└── README.md
```

---

## Setup & Installation

```bash
# Clone the repository
git clone https://github.com/shakeelahamed017/CrystallineAttachment.git
cd CrystallineAttachment

# Install dependencies
pip install -r requirements.txt

# Run the Flask API
python api/app.py
```

---

## Requirements

```
torch
transformers
scikit-learn
flask
numpy
pandas
Pillow
```

---

## About the Developer

**Shakeel Ahamed**
MCA Graduate — B.S. Abdur Rahman Crescent Institute of Science and Technology

- 📧 shakeelahamed7824@gmail.com
- 💼 [LinkedIn](https://www.linkedin.com/in/shakeel-ahamed-161354234)
- 🔐 Interests: NLP, Cybersecurity, Low-Code Development

---

## Status

> ✅ Project completed as part of MCA final year dissertation.

---

*Built with Python, HuggingFace Transformers, and Flask.*
