# Pneumatic/Hydraulic Brake Anomaly Detection - Edge Model
This module tracks pressure drops, friction-induced thermal patterns, and leakage vulnerabilities inside the critical braking mechanics.

## 📊 Dataset Reference
The model utilizes real-world high-cadence air compressor and pressure system logs. Download the source files here:
* **MetroPT3 Air Compressor Dataset:** [Kaggle Dataset Link](https://www.kaggle.com/datasets/nargesdavari/metropt3-air-compressor)
* **Focus Features:** Air pressure drops (`TP2`, `TP3`), motor current draw (`H1`), and ambient/oil operating temperatures to isolate mechanical seal leaks or sticking pads.

## 🔬 Edge Context Strategy
To protect the local vehicle power rail, this module executes conditional selective inference: the diagnostic calculations run dynamically only when brake system signals or active driver inputs are asserted.
