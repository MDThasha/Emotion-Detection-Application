# Emotion Voice Recognition System

## Overview
Emotional literacy is closely connected to, and often used interchangeably with, Emotional Intelligence (EQ). As both refer to the ability to recognize, understand, regulate and appropriately respond to emotions in oneself and in others. With the rise in rates for anxiety, depression and other mental health diagnoses, it has been studied to be more apparent in those with lower EQ scores than in those with high EQ scores. 

This project aims to develop an Emotion Voice Recognition System that has the ability of analysing human vocal signatures such as tone, pitch, rhythm and speech patterns to determine exactly what emotions are being exhibited at the given moment. With the goal being to bring about non-invasive mental health monitoring, and raise emotional literacy rates in future generations.

---

## 📑 Content
1. **Introduction**  
   1.1 Project Description  
   1.2 Purpose  
   1.3 Scope and Deliverables  
   1.4 Objectives

2. **Background Research**  
   2.1 Literature Review  
   2.2 Existing Systems  
   2.3 Technical Research  
      2.3.1 Why Voice-Based Emotion Detection?  
      2.3.2 Acoustic Features in Emotion Detection  
      2.3.3 How Emotions Differ Acoustically  
      2.3.4 Dataset Selection  
      2.3.5 Model Options  
      2.3.6 Platforms

---

# 1.0 Introduction
Anxiety, Depression, Intermittent Explosive Disorder (severe anger) and other mental health diagnoses have often been closely connected to the lack of Emotional Literacy or low Emotional Intelligence (EQ). As many individuals struggle to identify, understand and regulate their own emotional states, often due to difficulty in interpreting internal and external cues. This highlights the growing need for accessible tools that support emotional literacy, and self-awareness for early intervention to combat the ever rising growth of mental health diagnoses. Since vocal expression is one of the strongest indicators of emotional state, the integration of technology that analyses speech patterns offers a valuable and non-invasive method for detecting emotional changes in real time. 

---

## 1.1 Project Description
The Project aims to create an AI model that can detect various different emotions (happiness, sadness, anger, anxiety, and more) being exhibited from human speech by analyzing vocal audio features such as tone, pitch, rhythm and speech patterns. A Mix of the Ryerson Audio-Visual Database of Emotional Speech and Song (RAVDESS) and Crowd Sourced Emotional Multimodal Actors Dataset (CREMA-D) dataset will be used in this project to train the model to identify and differentiate between different emotions via audio waves while filtering background noises to maintain accuracy.

The project will incorporate a working application for real-time emotion recognition and an interactive learning component, where users can input their own vocal recordings to train emotional tone and speech control or listen to pre-recorded emotional samples to understand how different emotions sound.

With the main application of the system being in mental health monitoring, where voice-based emotion detection can offer non-invasive support and early intervention to the prevention and or the escalation of severe anxiety, depression, anger and other mental health diagnoses by promoting self-awareness, empathy, and emotional literacy.

---

## 1.2 Purpose
The purpose of this project is to train multiple working models with CREMA-D and RAVDESS dataset to accurately detect and identify different emotions simply through vocal audio alone. The best performing and most accurate model will be picked and used to create an application to implement certain features such as: Input audio so users can train manipulation on emotions in tone and speech with the application giving users feedback. Output of different emotional audio for user reference on what each emotion would sound like. 

Real-time emotion detection with live probability in the applications interface for each speaker (55% neutral and 45% anxiety). The application will also alert users when negative emotions such as anxiety or anger rise to critical levels, reminding them to pause, breathe, or calm down before continuing on what they were doing. Helping self regulation and understanding.

---

## 1.3 Scope and Deliverables
### **Technical Deliverables**
- Train 5 machine learning models using MFCC-extracted features:
  - Convolutional Neural Network (CNN)
  - Long Short-Term Memory (LSTM)
  - Support Vector Machine (SVM)
  - Recurrent Neural Network (RNN)
- Compare model performance and select the best one.
- Develop a Python-based GUI for real-time emotion recognition.
- Document challenges and limitations.

### **Project Management Deliverables**
- Provide consistent updates to the supervisor and client on the progress made each month.
- Amend the project to the clients needs and requirements each time they are requested.
- Produce Interim and Final reports on the project that covers every aspect of the project.


### **Out of Scope**
- Diagnosing mental health conditions.
- Clinical psychological analysis.

---

## 1.4 Objectives
- Support mental health monitoring through real-time detection.
- Reduce rising mental health diagnoses through early intervention.
- Encourage emotional literacy and self-awareness.

---

# 2.0 Background Research
Technology provides new opportunities for emotional development and mental health support. While many AI systems detect emotions through facial or physiological cues, few focus exclusively on **voice-based emotion detection** for emotional literacy.

---

## 2.1 Literature Review
Since the 2019 pandemic:
- Global EQ has dropped **5.78%**.  
- Anxiety and depression increased by **25%**.  
- 12% of the global population experiences anxiety or depression.  
- Anger and aggressiveness have risen significantly.

Studies consistently show that higher EQ correlates with better emotional stability, health, and coping skills. Emotional literacy remains difficult to teach in traditional education, creating a gap technology can fill.

---

## 2.2 Existing Systems
Several voice-based emotion recognition (SER) systems exist, mainly for HCI or clinical risk detection.

Examples include:
- Andrzej Majkowski — emotion analysis for HCI
- Kadiri — neutral emotion detection
- Alaa Nfissi — suicide prevention SER system

This project differs by focusing on improving emotional literacy and supporting everyday mental health through interactive learning.

---

## 2.3 Technical Research
“The Big Six,” used by Ekman et al (1969), which describes the six core emotions commonly exhibited by humans, Happiness, Anger, Sadness, Fear, Disgust, and Surprise. Today these core emotions are used universally by psychologists everywhere. Many datasets would contain at least 5 of these emotions in them in addition to any others.

### 2.3.1 Why Voice-Based Emotion Detection?
Research shows that **tone of voice** is one of the most reliable emotional indicators. Voice-only communication yields higher empathic accuracy than visual or multi-sensory communication. Emotions are harder to conceal through speech, making voice a strong foundation for machine learning.

### 2.3.2 Acoustic Features in Emotion Detection
Key features used:
- **Energy** — loudness changes
- **MFCCs** — spectral emotion cues
- **Zero-Crossing Rate** — voicing levels
- **Formants** — vocal tract resonance
- **F0 (Pitch)** — emotional intensity

### 2.3.3 How Emotions Differ Acoustically
- **High arousal** (Anger, Happiness): high energy, pitch variation, distinct MFCCs
- **Medium arousal** (Fear, Surprise)
- **Low arousal** (Sadness, Neutral): low energy, subtle changes
- Disgust is the most inconsistent and hardest to detect

Focus emotions: **Happiness, Sadness, Anger, Fear, Neutral**.

### 2.3.4 Dataset Selection
Comparison (summary):
- **CREMA-D**: 7.4k samples, 91 speakers, 6 emotions, open licence
- **RAVDESS**: 1.4k samples, 24 speakers, 8 emotions, open licence
- Others (IEMOCAP, SAVEE, TESS) have licensing or diversity limitations

Chosen datasets: **CREMA-D + RAVDESS**.

### 2.3.5 Model Options
- **CNN** — learns spectral patterns
- **LSTM** — learns temporal emotion patterns
- **RNN** — simple sequence modelling
- **SVM** — strong baseline for MFCC-based classification

### 2.3.6 Platforms
- **Python** for all development
- **Jupyter Notebook** for training, data visualisations and experimentation
- **Windows** as deployment platform for GUI application

---
