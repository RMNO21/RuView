# RuView RF Sensing Architecture

## 1. Overview
RuView extracts spatial intelligence and human motion telemetry from commodity Wi-Fi Channel State Information (CSI) signals without optical sensors.

## 2. Core Signal Processing Pipeline
1. **Raw Frame Ingestion**: Capturing 802.11 raw frame headers and CSI matrices from edge nodes (ESP32 / Wi-Fi NICs).
2. **Phase Sanitization**: Unwrapping phase angles and removing Carrier Frequency Offset (CFO) and Sampling Frequency Offset (SFO).
3. **Filtering & Decomposition**: Butterworth bandpass filtering (0.1 - 0.5 Hz) and Principal Component Analysis (PCA) for sensitive subcarrier isolation.
4. **Motion Classification**: Time-series feature extraction for vital signs and presence detection.
