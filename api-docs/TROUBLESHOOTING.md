# RuView Diagnostics & RF Troubleshooting

## 1. High Phase Noise on 2.4 GHz
- **Cause**: 2.4 GHz band congestion and Bluetooth coexistence interference.
- **Remedy**: Switch to 5 GHz UNII-1 channels with 40MHz channel width or use isolated test environments.

## 2. Packet Dropouts on Edge Nodes
- **Cause**: Buffer saturation on low-memory microcontrollers (e.g., ESP32 WROOM).
- **Remedy**: Enable DMA for SPI/Wi-Fi buffers and throttle sampling rate to 100 Hz.
