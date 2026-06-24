# Motor/Engine Health Diagnostic - Edge Model
This module handles high-frequency vibration feature extraction and structural bearing anomaly detection for the electric powertrain.

## 📊 Dataset Reference
The model is trained on standard industrial bearing and vibration benchmark logs. Download the source files here:
* **CWRU Bearing Dataset (Case Western Reserve University):** [Kaggle Dataset Mirror](https://www.kaggle.com/datasets/astrollama/cwru-case-western-reserve-university-dataset) or the [Official CWRU Data Repository](https://engineering.case.edu/bearingdata-center).
* **Focus Features:** High-frequency digital accelerometer data (Drive End and Fan End data columns).

## 🔬 Feature Engineering Strategy
Because raw vibration time-series data is highly volatile, this sub-module utilizes:
1. **Time-Domain:** Root Mean Square (RMS) and Kurtosis tracking to detect mechanical impacts.
2. **Frequency-Domain:** Fast Fourier Transform (FFT) to monitor localized peak frequency shifts in rotating components.
