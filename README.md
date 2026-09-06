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

| Technology / Concept         | Purpose                   |
| ---------------------------- | ------------------------- |
| 🟠 **Scilab**                | DSP implementation        |
| 🎧 **WAV Audio**             | Input and output signals  |
| 🔧 **Moving Average Filter** | Noise reduction           |
| 📊 **FFT**                   | Frequency-domain analysis |
| 📈 **Time-Domain Analysis**  | Waveform visualization    |
| 📉 **SNR**                   | Performance evaluation    |

| Parameter          |              Value |
| ------------------ | -----------------: |
| Sampling Frequency |         **16 kHz** |
| Number of Samples  |         **20,432** |
| Noise Amplitude    |            **0.1** |
| Filter Type        | **Moving Average** |
| Filter Window Size |              **3** |
| Signal Type        |   **Speech Audio** |

🔬 How It Works

1️⃣ Load the Audio

The original speech audio signal is loaded from a WAV file and represented as a sequence of digital samples.

The audio used in this project has a sampling frequency of 16 kHz.

2️⃣ Generate Noise

Artificial zero-mean random noise is generated and added to the original audio signal.

Noisy Signal = Clean Signal + Noise

The noise amplitude used in this project is:0.1

3️⃣ Apply Moving Average Filter

A Moving Average Filter is applied to the noisy signal.

For a window size of M = 3:y[n] = (x[n] + x[n-1] + x[n-2]) / 3

The filter averages neighboring samples to smooth rapid variations in the signal.

4️⃣ Time-Domain Analysis

The clean, noisy and filtered audio signals are plotted in the time domain.

This allows the waveform changes caused by noise and filtering to be visually compared.

5️⃣ Frequency-Domain Analysis

The Fast Fourier Transform (FFT) is used to analyze the frequency components of the audio signal.

The project compares the frequency spectra of:

Clean audio
Noisy audio
Filtered audio

This helps demonstrate how the signal changes in the frequency domain after filtering.
6️⃣ SNR Analysis

The Signal-to-Noise Ratio (SNR) is calculated before and after filtering to evaluate the filtering process.

Results       Measurement	Result
SNR Before Filtering	≈ 9.69 dB
SNR After Filtering	≈ 8.89 dB
SNR Change	≈ -0.80 dB

📌 Observation

For this particular test signal and filter configuration, the measured SNR decreased slightly after filtering.

This happens because the simple Moving Average Filter can reduce some unwanted variations while also introducing signal distortion.

This result demonstrates an important DSP concept:"Effective noise reduction depends on selecting an appropriate filter and suitable parameters for the characteristics of the signal and noise."

📊 Signal Comparison

The project processes and compares three main signals:

🎵 Clean Signal

The original speech audio signal.

🔊 Noisy Signal

The original signal after artificial random noise is added.

🎧 Filtered Signal

The noisy signal after applying the Moving Average Filter.

The signals are compared in both the time domain and frequency domain.

📁 Project Structure
Audio_Noise_Reduction/
│
├── 📂 audio/
│   └── 🎵 clean_audio.wav
│
├── 📂 scilab/
│   └── 📄 main.sce
│
└── 📂 results/
    ├── 🔊 noisy_audio.wav
    └── 🎧 cleaned_audio.wav

▶️ How to Run
Requirements
Scilab
WAV audio file
Steps
Download or clone this repository.
Install Scilab.
Open the project in Scilab.
Open scilab/main.sce.
Run the program.
Observe the generated signal plots.
Analyze the FFT frequency spectra.
Check the calculated SNR values.
Listen to the generated audio files.
Generated Output
The program generates:
results/
│
├── noisy_audio.wav
└── cleaned_audio.wav

🧠 DSP Concepts Learned

Through this project, I gained practical understanding of:

Digital audio signals
Sampling frequency
Signal amplitude
Random noise
Time-domain representation
Frequency-domain representation
Fast Fourier Transform (FFT)
Moving Average Filtering
Signal-to-Noise Ratio
Audio signal processing
Signal distortion caused by filtering
Basic DSP implementation using Scilab

🚀 Future Improvements

The project can be further improved by implementing:

🔧 FIR Low-Pass Filters
🔧 IIR Filters
🎚️ Different filter window sizes
📊 Spectrogram analysis
🎵 Different types of noise
⚡ Frequency-domain noise reduction
🔬 Comparison of multiple filtering techniques
🎙️ Real-time audio noise reduction

🎯 Project Goal

The main goal of this project was to gain practical experience in Digital Signal Processing by moving from theoretical concepts to the processing of an actual audio signal.

This project provides a foundation for exploring more advanced audio processing and DSP techniques.

---

## 👨‍💻 Author

### Purushotam Joshi

Electronics & Communication Engineering  
SUIET

---

⭐ If you found this project useful, consider giving the repository a star!
