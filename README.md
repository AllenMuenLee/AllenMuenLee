# Allen Lee (Mu-En Lee)

Researching hybrid quantum–classical recurrent architectures for sequence modeling and time-series forecasting.

---

## Featured Research

### [Q-sLSTM — Quantum Scalar Long Short-Term Memory](https://github.com/AllenMuenLee/Q-sLSTM)

[![GitHub Repo](https://img.shields.io/badge/GitHub-AllenMuenLee%2FQ--sLSTM-181717?style=flat&logo=github)](https://github.com/AllenMuenLee/Q-sLSTM)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![PennyLane](https://img.shields.io/badge/PennyLane-19B37B?style=flat)

Quantum extension of scalar LSTM (sLSTM / xLSTM) replacing classical gate projections with four independent Variational Quantum Circuits (VQCs) and stabilized amplified gating.

- **Stabilized Quantum Recurrence:** Combines amplified input/forget gating with xLSTM-style normalized state updates `(h, c, n, m)` and binary-scaled state tracking to prevent overflow across long sequences.
- **Gate Formulations:** Implements paired-seed comparisons across odds-ratio gates `(1 + q) / (1 - q)` (`qslstm`), square-root gates `sqrt((1 + q) / (1 - q))` (`qslstm_sqrt`), and float64 logarithmic gates `ln(2 / (1 - q))` (`qslstm_log`), alongside standard `qlstm` and classical baselines.
- **Benchmarking & Extrapolation:** Full reproducible suites spanning 1-D recurrent memory probes (`delay`, `ema`, `running_max`, `flip_flop`, `narma`, `sine_next`), nearest-neighbor memory revision, weather stations, and solar generation forecasting.

---

### [Recursive QLSTM — Stable Short-Horizon Temperature Forecasting](https://arxiv.org/abs/2609.20594)

[![arXiv](https://img.shields.io/badge/arXiv-2609.20594-B31B1B?style=flat&logo=arxiv&logoColor=white)](https://arxiv.org/abs/2609.20594)

> **Recursive Quantum Long Short-Term Memory for Stable Short-Horizon Temperature Forecasting**
> **Mu-En Lee**, Yen-Ku Liu, Samuel Yen-Chi Chen, Yun-Cheng Tsai *(arXiv:2609.20594, 2026)*

- **Motivation:** Standard QLSTM optimization can vary substantially across random initializations and temporal contexts.
- **Approach:** Evaluates a recursive QLSTM architecture with recursive quantum feature/parameter transformations against standard QLSTM under identical training settings.
- **Key Findings:** Across 8-, 16-, and 32-day input windows over 20 random seeds on daily min/max Toronto temperature forecasting, Recursive QLSTM reaches near-optimal test loss earlier, reduces MAE and RMSE, and narrows the generalization gap.

---

## Core Focus

- **Quantum Machine Learning:** Variational Quantum Circuits (VQCs), PennyLane, PyTorch hybrid training
- **Recurrent Architectures:** Q-sLSTM, Recursive QLSTM, QLSTM, xLSTM / sLSTM memory stabilization
- **Sequence Modeling:** Short- and long-horizon time-series forecasting, memory revision, and dynamical systems

---

<details>
<summary><strong>Other Side Projects</strong> (Hardware, Systems &amp; Tooling)</summary>

<br>

| Project | Stack | Summary |
| --- | --- | --- |
| [FPGAudio-Sound-Board](https://github.com/AllenMuenLee/FPGAudio-Sound-Board) | SystemVerilog | Real-time audio DSP engine on Intel Cyclone V (DE1-SoC) interfacing directly with the WM8731 codec |
| [3D-Rendering-Engine](https://github.com/AllenMuenLee/3D-Rendering-Engine) | Verilog | Hardware 3D rendering pipeline implemented in RTL |
| [Citats](https://github.com/AllenMuenLee/Citats) | TypeScript / Python | AI-native desktop browser workspace with dynamic API discovery and generated UI |
| [TFX-Quant](https://github.com/AllenMuenLee/TFX-Quant) | Python | Automated futures trading desktop system with position and session risk limits |
| [Remote-AI-Agent](https://github.com/AllenMuenLee/Remote-AI-Agent) | TypeScript | Mobile-to-desktop bridge for controlling local CLI coding agents remotely |
| [Allen-IME](https://github.com/AllenMuenLee/Allen-IME) | C++ | Windows Input Method Editor (IME) with autocomplete support |

</details>
