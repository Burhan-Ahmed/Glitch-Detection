# Glitch Detection and Restoration of Noisy Sinusoidal Waveforms using MATLAB

A MATLAB project that analyzes a one-hour noisy sinusoidal audio recording, **pinpoints the exact moment a frequency glitch occurs**, removes the glitch, and then filters out the noise to restore a clean sine wave.

> Complex Engineering Activity, Digital Signal Processing, Department of Electrical & Computer Engineering, Air University (May 2024)

---

## Problem statement

Given a noisy sinusoidal waveform (`Noisy.wav`) that contains a glitch, build a MATLAB program that:

1. Plots the waveform against time
2. Finds the frequency content of the signal
3. Detects the precise time (hr:min:sec) at which the glitch occurs
4. Removes the glitch
5. Removes the noise

## Results

- **Glitch detected:** starts at `00:32:59.955`, ends at `00:33:05.997`
- **Glitch duration:** about 6.04 seconds
- Glitch smoothed with the FIR low-pass filter, and noise suppressed with the zero-phase Butterworth filter
- Output files: `improved_audio.wav` (glitch removed) and `Cleaned_Sinusoid.wav` (final denoised signal)


## How to run

1. Open **MATLAB** (developed with R2021a). The Signal Processing Toolbox is required for `spectrogram`, `fir1` and `butter`.
2. Put `Noisy.wav` in the working directory.
3. Run the scripts in order, from task 1 to task 5.
4. Listen to `improved_audio.wav` and `Cleaned_Sinusoid.wav` to hear the improvement.


This project was developed for academic purposes. Add a license of your choice (for example MIT) if you want others to reuse it.
