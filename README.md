# OFDM Simulation

Simulation of an OFDM transmitter and receiver using Python and Jupyter Notebook.

The project demonstrates OFDM signal generation, transmission through different channel conditions, receiver synchronization, and demodulation.

## View Online

[![View on GitHub](https://img.shields.io/badge/View-GitHub-24292F?logo=github)](https://github.com/nomatin/OFDM-Phy-Simulation/blob/main/ofdm.ipynb)
[![View in nbviewer](https://img.shields.io/badge/View-nbviewer-F37626?logo=jupyter&logoColor=white)](https://nbviewer.org/github/nomatin/OFDM-Phy-Simulation/blob/main/ofdm.ipynb)

## Run Online

[![Launch Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/nomatin/OFDM-Phy-Simulation/90d7493a43e42e7a938c4861643cfee602563726?urlpath=lab%2Ftree%2Fofdm.ipynb)

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

## Run Locally

From the repository root, use Python 3.11 or later to install the dependencies and open the notebook.

```bash
python -m pip install -r requirements.txt
python -m jupyterlab ofdm.ipynb
```

Set the simulation parameters in **OFDM, Modulation, and Channel Constants**, then run all cells from a fresh kernel.

## Simulation Results

### Effect of Additive Noise

![Waterfall spectrograms comparing the ideal channel with AWGN at 5 dB SNR](assets/effect-of-additive-noise.png)

Both spectrograms use the same power scale. The AWGN case uses 5 dB SNR and shows the noise floor around the OFDM burst.

### CFO and Pilot Phase Correction

![Received constellations before compensation, after CFO compensation, and after pilot phase correction](assets/cfo-and-pilot-phase-correction.png)

The channel applies AWGN at 5 dB SNR and a carrier frequency offset of 960 Hz. The receiver estimates CFO from the cyclic prefix and compensates the phase drift within each symbol. It then uses the pilots to align the constellation across symbols.
