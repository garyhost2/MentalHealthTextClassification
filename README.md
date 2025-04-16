<div align="center">

# 🧠 MindScope  
### 5th Place Solution — GODS Hackathon 🥉

A Deep Learning approach for early detection of mental health conditions from text.

[![View the Project](https://img.shields.io/badge/View%20Project-GitHub-black?logo=github)](https://github.com/garyhost2/MentalHealthTextClassification)

</div>

---

## 🧩 Overview

**MindScope** is a text classification solution developed during the **GODS Hackathon**, hosted by the IEEE ENSI Student Branch and the IEEE ENSI CIS Chapter.

In today’s digital age, countless individuals share their mental health experiences online. Our model leverages this data to **identify early signs of depression, anxiety, and relationship issues** through Natural Language Processing (NLP), aiming to provide a foundation for **early intervention and mental health support**.

---

## 🧠 Problem Statement & Objective

- **Goal**: Classify user-generated text into relevant mental health topics.  
- **Why It Matters**: Early detection can save lives by enabling timely support.
- **Metric**: **Accuracy** – classification performance on provided data.

---

## 🏗️ Model Architecture

<p align="center">
  <img src="https://i.postimg.cc/NFPwd7C8/Neuro-Pulse-AI-Powered-Mental-Wellness-Scanner.png" width="400"/>
</p>

### ✍️ Workflow Summary:
- Concatenated title and content → dataset preprocessing  
- **GPT-2** used for **data augmentation**  
- Fine-tuning on multiple models:
  - RoBERTa-Base & RoBERTa-Large  
  - DeBERTa V3 Base  
- **Majority Voting Ensemble** for final predictions  
- Longformer planned but not finalized due to time/resources

---

## 📊 Dataset Format

- **Input**: CSV with two fields – `ID` and `Text`  
- **Output**: CSV file with the following format:
  ```csv
  ID,Label
  1,Anxiety
  2,Depression
  ...
