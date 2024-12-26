# SPA for LDPC Codes

This project This project implements the **Sum Product Algorithm (SPA)** for decoding **Low-Density Parity-Check (LDPC)** codes. It includes encoding, decoding, and performance analysis for LDPC codes over noisy communication channels. It was developed by me during my Master's studies at Skoltech University, Skolkovo, Russia.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [License](#license)

## Introduction
Low-Density Parity-Check (LDPC) codes are a powerful class of error-correcting codes used in modern communication systems. The Sum Product Algorithm (SPA) is an iterative message-passing algorithm employed to decode LDPC codes. This project demonstrates the application of SPA with examples of performance evaluation under varying Signal-to-Noise Ratios (SNRs).

## Features
- Belief Propagation (SPA): Implements SPA for decoding LDPC codes.
- Encoding and Decoding: Simulates communication over noisy channels.
- BER and FER Analysis: Evaluates Bit Error Rate (BER) and Frame Error Rate (FER) for multiple SNR values.
- Visualization: Includes plots for BER and FER performance across SNRs.

## Dependencies
The project is implemented in Python and uses the following libraries:
- `numpy`
- `matplotlib`

Install dependencies using:
```bash
pip install numpy matplotlib
```

## Usage
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/spa-for-ldpc.git
    cd spa-for-ldpc
    ```
2. Open the Jupyter Notebook `ICT_Project_SPA_for_LDPC.ipynb`:
    ```bash
    jupyter notebook ICT_Project_SPA_for_LDPC.ipynb
    ```
3. Run the cells step-by-step to:
   - Load the MNIST image data.
   - Simulate encoding and decoding using SPA.
   - Analyze performance metrics (BER and FER).
   - Visualize results.

## Project Structure
- `ICT_Project_SPA_for_LDPC.ipynb`: Main notebook with code, documentation, and visualizations.
- Simulation examples for:
  - Single SNR value (2.5 dB).
  - Multiple SNR values for BER and FER evaluation.
- Plots generated using `matplotlib`.

## License
This project is licensed under the MIT License. Feel free to use and modify the code.

