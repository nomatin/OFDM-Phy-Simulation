# OFDM Simulation

Simulation of an OFDM transmitter and receiver using Python and Jupyter Notebook.

The project demonstrates OFDM signal generation, transmission through different channel conditions, receiver synchronization, and demodulation.

[Open ofdm.ipynb in nbviewer](https://nbviewer.org/github/nomatin/OFDM-Phy-Simulation/blob/main/ofdm.ipynb)

## Features

- OFDM modulation and demodulation
- Configurable OFDM parameters
- Data and pilot subcarrier allocation
- Cyclic prefix insertion and synchronization
- AWGN and carrier frequency offset (CFO) simulation
- CFO estimation and compensation
- Pilot-based phase correction
- Bit Error Rate (BER) analysis
- Signal spectrum, spectrogram, and constellation visualization

## Requirements

- Python 3
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook or JupyterLab

## Usage

Install dependencies:

```bash
pip install numpy scipy matplotlib jupyterlab
```

Open `ofdm.ipynb` in JupyterLab.

Simulation parameters can be changed in the **OFDM, Modulation, and Channel Constants** section.

Run the notebook cells sequentially to generate signals, simulate the channel, and analyze the receiver results.
