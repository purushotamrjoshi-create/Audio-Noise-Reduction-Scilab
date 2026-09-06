<div align="center">

# 🎧 Audio Noise Reduction System

### Digital Signal Processing Mini Project using Scilab

<p>
  <b>Analyze • Add Noise • Filter • Compare • Evaluate</b>
</p>

<br>

![Scilab](https://img.shields.io/badge/Scilab-DSP-orange?style=for-the-badge)
![DSP](https://img.shields.io/badge/Digital%20Signal%20Processing-blue?style=for-the-badge)
![Audio](https://img.shields.io/badge/Audio%20Processing-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

</div>

---

## 📌 About the Project

**Audio Noise Reduction System** is a beginner-level **Digital Signal Processing (DSP)** project developed using **Scilab**.

The project demonstrates the basic process of adding artificial noise to a speech signal and applying a **Moving Average Filter** to reduce unwanted variations.

The system also analyzes the signal in both the **time domain** and **frequency domain** using the **Fast Fourier Transform (FFT)** and evaluates the filtering process using **Signal-to-Noise Ratio (SNR)**.

---

## ✨ Key Features

- 🎵 WAV audio signal processing
- 📢 Artificial noise generation
- 🔊 Noisy audio creation
- 🔧 Moving Average filtering
- 📈 Time-domain signal visualization
- 📊 Frequency-domain analysis using FFT
- 📉 SNR calculation
- 💾 Processed audio output
- 🔍 Comparison of clean, noisy and filtered signals

---

## 🔄 Processing Workflow

```text
             🎵 CLEAN AUDIO
                    │
                    ▼
          ┌──────────────────┐
          │  Noise Generation │
          └────────┬─────────┘
                   │
                   ▼
             🔊 NOISY AUDIO
                   │
                   ▼
          ┌──────────────────┐
          │ Moving Average   │
          │     Filter       │
          └────────┬─────────┘
                   │
                   ▼
          🎧 FILTERED AUDIO
                   │
          ┌────────┴────────┐
          ▼                 ▼
   📈 Time Domain     📊 Frequency Domain
      Analysis            Analysis
          │                 │
          └────────┬────────┘
                   ▼
              📉 SNR Analysis
