---
title: "EE430 Digital Signal Processing Course Project 2023-2024 "
excerpt: "AUVSI SUAS is an annual competition that challenges student teams to design, build, and operate unmanned aerial vehicles (UAVs or drones). The competition typically involves a series of missions that test the capabilities of the teams' autonomous systems. These missions often include tasks such as autonomous flight, target identification, and payload delivery.<br/><img src='/images/dsp.png'>"
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
