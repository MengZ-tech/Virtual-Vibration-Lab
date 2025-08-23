# Virtual-Vibration-Lab

> ⚙️ Make the time-domain signal as you wish, and **see what happens in the frequency domain**.

<p align="center">
  <a href="https://mengz-tech.github.io/Virtual-Vibration-Lab/">
    <img alt="hero" src="https://github.com/user-attachments/assets/38a6ca36-9783-4d89-9832-5bece07f66e8" width="92%">
  </a>
</p>

<p align="center">
  <a href="https://mengz-tech.github.io/Virtual-Vibration-Lab/">Live Demo</a> ·
  <a href="#features">Features</a> ·
  <a href="#how-it-works">How it works</a> ·
  <a href="#gallery">Gallery</a> ·
  <a href="#references">References</a>
</p>

<p align="center">
  <img alt="Static Badge" src="https://img.shields.io/badge/Signals-Vibration-blue">
  <img alt="Static Badge" src="https://img.shields.io/badge/FFT-Analysis-informational">
  <img alt="Static Badge" src="https://img.shields.io/badge/Envelope-Demodulation-success">
  <img alt="Static Badge" src="https://img.shields.io/badge/License-MIT-lightgrey">
</p>

---

## Features

- 🎛️ **Direct control** of impulses, carriers, envelopes, and noise.
- ✏️ **Draw your own envelope** and see spectrum changes in real time.
- 📡 **Random shock-arrival jitter** to visualize spectral broadening / smearing.
- 🧭 **Compare** time vs. (envelope) spectrum side-by-side.

---

## Live Demo

> Open in browser

**🔗 https://mengz-tech.github.io/Virtual-Vibration-Lab/**

---

## How it works

- Time-domain signal = (carrier / baseband) × envelope + noise.
- Envelope can be parametric **or** hand-drawn.
- FFT of the raw signal shows harmonic content;  
  FFT of the **envelope / demodulated** signal highlights modulation and sidebands.
- **Shock-arrival jitter** perturbs event times → frequency-domain **broadening**.

---

## Gallery

### Create your own envelope — draw it and observe spectral impact
<p align="center">
  <img alt="env" src="https://github.com/user-attachments/assets/4611c76c-3e93-4aab-90ea-72f8df0538b1" width="40%">
</p>

### Sidebands from envelope modulation
<p align="center">
  <img alt="sideband" src="https://github.com/user-attachments/assets/6591f55c-0b5c-45aa-9cbe-9420d321d8df" width="80%">
</p>

### Random shock-arrival jitter → FFT effects
<p align="center">
  <img alt="jitter-1" src="https://github.com/user-attachments/assets/3c0b16bb-e8b3-4eaa-821a-47c3702360b7" width="80%">
  ![1](https://github.com/user-attachments/assets/44b69f7d-febc-4640-aacf-619241a66f33)

</p>
<p align="center">
  <img alt="jitter-2" src="https://github.com/user-attachments/assets/ff5032ec-cd7c-41f4-b082-cfd3a8ce6a34" width="80%">
</p>
<p align="center">
  <img alt="jitter-3" src="https://github.com/user-attachments/assets/f0dd19b3-abd2-4459-821a-47c3702360b7" width="80%">
</p>

---

## Tips

- Start with a **simple periodic impulse train**, then add an envelope to watch **sidebands** emerge.
- Another thing I want to mention is to illustrate how the shock arrival time (or, would you call it Uncertainty?) influences the Fourier spectrum (which is quite a common case in the real world). Use "random jitter (of the shock arrival time)" button to see the effect on FFT results, but also be aware that this "random jitter" may not be the most accurate model when it comes to components like bearings. check: FDS-MOMEDA: optimization-blind deconvolution in finite high-dimensional spaces for extracting pulse signal in rolling bearing fault diagnosis. Measurement Science and Technology, 35(8), 086140. https://doi.org/10.1088/1361-6501/ad4dcb

