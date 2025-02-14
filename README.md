# Communication Systems Coursework and Final Project

This repository contains implementations of various **analog and digital communication system techniques** and simulations. The work is divided into coursework files (`chw1`, `chw2`, `chw3`) and a final project.

---

## Coursework Files (`chw1`, `chw2`, `chw3`)
In these files, I have implemented and simulated various analog and digital communication system techniques, including but not limited to:
- Modulation and demodulation techniques
- Signal processing methods
- Noise analysis and mitigation
- Channel simulations

---

## Final Project: Image Transmission System

### Overview
In this project, we design and analyze a **digital communication system for image transmission**. The system consists of multiple processing stages, including:
1. **Image Preprocessing**: Preparing the image for transmission.
2. **Modulation**: Converting the data into a transmittable signal.
3. **Channel Transmission**: Simulating the transmission through a noisy channel.
4. **Equalization**: Mitigating inter-symbol interference (ISI).
5. **Reconstruction**: Recovering the original image from the received signal.

### System Design
1. **Image Compression**:
   - The image is compressed using **Discrete Cosine Transform (DCT)** into quantized blocks.
   - The quantized coefficients are converted into a bitstream.

2. **Modulation**:
   - The bitstream is modulated using **Pulse Amplitude Modulation (PAM)**.
   - Two pulse shapes are compared:
     - **Half-Sine**
     - **Square Root Raised Cosine (SRRC)**

3. **Channel Transmission**:
   - The modulated signal is transmitted through a **linear time-invariant (LTI) channel** with **additive white Gaussian noise (AWGN)**.

4. **Receiver Processing**:
   - The received signal is passed through a **matched filter**.
   - **Equalization** is performed using:
     - **Zero-Forcing (ZF) Equalizer**
     - **Minimum Mean Square Error (MMSE) Equalizer**
   - The recovered bitstream is used to reconstruct the original image using **inverse DCT**.

### Testing and Validation
1. **Component Testing**:
   - Individual components (e.g., modulation, equalization) are tested using a sequence of **10 random bits** to verify functionality.

2. **System Testing**:
   - The complete system is applied to transmit and reconstruct an image.
   - Performance is analyzed under different conditions, such as:
     - **Noise levels**
     - **Channel distortions**

---

## Repository Structure
