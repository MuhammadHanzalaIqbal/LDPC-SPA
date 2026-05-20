# LDPC-SPA

**Sum-Product Algorithm (SPA) decoder for Low-Density Parity-Check (LDPC) codes — encoding, soft-information decoding, and BER/FER performance analysis over an AWGN channel.**

A Python implementation of belief-propagation / sum-product decoding for LDPC codes. The simulation evaluates LDPC-coded transmission over a noisy channel: encode → AWGN channel → SPA decoder → BER and FER curves across SNR.

## What this project does

- **Encoding:** systematic LDPC encoder using a parity-check matrix `H`.
- **Channel:** additive white Gaussian noise with parameterizable SNR (Eb/N0).
- **Decoding:** iterative **Sum-Product Algorithm** (a.k.a. belief propagation) operating on the Tanner graph of `H`. Soft log-likelihood-ratio messages are exchanged between variable nodes and check nodes; iterations continue until convergence or a max-iter cap.
- **Evaluation:**
  - **BER** (Bit Error Rate) and **FER** (Frame Error Rate) measured across a sweep of SNR values.
  - A single-SNR (2.5 dB) detailed run as a sanity-check waterfall point.
  - Full multi-SNR sweep to draw the canonical BER-vs-SNR curve.
- **Visualization:** BER/FER vs SNR curves with `matplotlib`.

## What's in here

| File | Purpose |
|---|---|
| `Project.rar` | Python source (`.ipynb` + helpers) — extract before running |
| `ICT_SPA.pdf` | Written project report |
| `README.md` | This document |

## Running it

After extracting `Project.rar`:

```bash
pip install numpy matplotlib
jupyter notebook ICT_Project_SPA_for_LDPC.ipynb
```

Run cells in order: encoding setup → SPA decoder definition → single-SNR demo → BER/FER sweeps → plots.

## Context

Academic project developed during M.Sc. studies at the **Skolkovo Institute of Science and Technology (Skoltech)**. Sits in the same digital-communications portfolio as [`Channel-Estimation`](https://github.com/MuhammadHanzalaIqbal/Channel-Estimation), [`mimo-channel-estimation`](https://github.com/MuhammadHanzalaIqbal/mimo-channel-estimation), and [`mimo-channel-denoising`](https://github.com/MuhammadHanzalaIqbal/mimo-channel-denoising).

---

*Author: Muhammad Hanzala Iqbal.*
