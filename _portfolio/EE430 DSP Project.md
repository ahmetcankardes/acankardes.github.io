---
title: "EE430 Digital Signal Processing Course Project 2023-2024 "
excerpt: "AUVSI SUAS is an annual competition that challenges student teams to design, build, and operate unmanned aerial vehicles (UAVs or drones). The competition typically involves a series of missions that test the capabilities of the teams' autonomous systems. These missions often include tasks such as autonomous flight, target identification, and payload delivery.<br/><img src='/images/dsp.png' width='600' height='450'>"
collection: portfolio
---


# EE430 Term Project Part 1

## Overview
This project, conducted in collaboration with my friend [Hasan Hüseyin Karatas](https://www.linkedin.com/in/hasan-huseyin-karatas/), is part of the EE430 Digital Signal Processing course at METU's Department of Electrical and Electronics Engineering. The objective of Part 1 is to implement a computer program that computes and displays the magnitude of the short-time Fourier transform (STFT) of a signal.

## Project Description

### Short-Time Fourier Transform (STFT)
The STFT, discussed in Chapter 10 of the course's textbook (Discrete-time Signal Processing 3rd ed. Oppenheim, Schafer Pearson, 2010.), is a sequence of Fourier transforms applied to short consecutive segments of a long signal. It is useful for analyzing the temporal frequency content of a signal, often referred to as "Time Dependent Fourier Transform."

### Tasks

#### Data Acquisition
The implemented program can work with various input signals:
- Sound data from a microphone: Captures user voice or audio playback with an adjustable sampling rate.
- Sound data from a file: Processes .wav or .mp3 files, retrieving time-domain signals and sampling frequencies.

#### Data Generation
The system generates time-domain signals using simple mathematical expressions. Examples include sinusoidal signals and windowed sinusoidal signals with adjustable parameters.

#### Spectrogram
A MATLAB code is written to display the spectrogram of a discrete-time signal. This spectrogram is a plot of the magnitude of the STFT on the time-frequency plane, providing insights into the signal's temporal frequency content.

### Implementation and Deliverables
A graphical user interface (GUI) is created using MATLAB's app designer to facilitate data acquisition, data generation, and spectrogram visualization. The GUI allows users to adjust parameters such as sampling rate, amplitude, frequency, phase, and signal duration.

## Navigation to GitHub Page
For detailed MATLAB code and further project details, please refer to the GitHub repository

# EE430 Term Project Part 2

## Background

Signaling is the exchange of information using signals between network devices to manage communication sessions. One example is dialing a phone number, where dialed digits are transmitted to route the call correctly. In the past, rotary dialing was standard, but it was slow and inefficient. To address this, push-button dialing with dual-tone multi-frequency (DTMF) signaling was developed. Each key press generates a signal composed of two constant frequencies. Part 2 of the project involves experimenting with DTMF signaling.

### DTMF Encoding Formula

A DTMF-encoded key can be expressed as follows:
$s(k)(t; T_d) = (\sin(f_L(k)t) + \sin(f_H(k)t)) \cdot (u(t) - u(t - T_d))$
where:
- \(s\) is the time-domain signal corresponding to the pressed key,
- \(k\) is the index of the key,
- \(f_L(k)\) and \(f_H(k)\) are the respective low and high frequencies,
- \(T_d\) is the signaling duration per key.

### DTMF-encoded Sequence Formula

Given a discrete sequence of numbers \(x[n]\), the DTMF-encoded sequence \(m(t; T_d, T_r)\) can be expressed as:
\[m(t; T_d, T_r) = \sum s(x[k])(t - k(T_d + T_r); T_d) \quad \text{where} \quad k = 0, 1, \ldots, N-1\]
and \(T_r\) is the resting duration between two consecutively pressed keys.

## Deliverables

For all items, you are required to write MATLAB codes and design a graphical user interface (GUI) using the app designer.

### Transmitter Panel

- A push-button keypad,
- A display field to show pressed keys as text,
- A reset button to clear pressed keys,
- Input fields for signaling duration per key (\(T_d\)) and resting duration (\(T_r\)),
- An input field to adjust the amplitude of the time-domain signal,
- A time-domain signal panel to display the DTMF-encoded sequence \(m(t; T_d, T_r)\),
- Display of the spectrogram of the generated signal \(m(t; T_d, T_r)\),
- Save and play buttons for saving and playing the generated signal as audio.

### Receiver Panel

- Input fields for signaling duration per key (\(T_d\)) and resting duration (\(T_r\)),
- Start/stop listening button,
- A display to plot the received time-domain signal,
- A display to plot its spectrogram,
- A switch to select the decoding algorithm,
- A display field to show the decoded signal.

## Further Reading

For real-time displays, you can plot the signals at a separate figure from the GUI. You can also create checkbox elements to enable/disable plotting to balance the load on processing if needed.

For decoding the received signal, the user must be able to select between a spectrogram-based method and another algorithm of your choice.

• DTMF: https://en.wikipedia.org/wiki/Dual-tone_multi-frequency_signaling
• Signalling: https://en.wikipedia.org/wiki/Signaling_(telecommunications)
• Filter Banks: https://en.wikipedia.org/wiki/Filter_bank
• Goertzel algorithm: https://en.wikipedia.org/wiki/Goertzel_algorithm
• MUSIC algorithm: https://en.wikipedia.org/wiki/MUSIC_(algorithm)
• Real Time Audio: https://www.mathworks.com/help/audio/gs/real-time-audio-in-matlab.html
• Audio I/O Buffering: https://www.mathworks.com/help/audio/gs/audio-io-buffering-latency-andthroughput.html


## Navigation to GitHub Page

For detailed MATLAB code and further project details, please refer to the GitHub repository.

