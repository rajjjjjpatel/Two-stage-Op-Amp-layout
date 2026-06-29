# Two-Stage CMOS Operational Amplifier Layout

This repository contains the complete layout implementation of a **Two-Stage CMOS Operational Amplifier** designed using the Cadence Virtuoso design flow. The project includes schematic design, layout generation, physical verification, parasitic extraction, and post-layout performance evaluation.

## Project Overview

The objective of this project is to design and verify a two-stage CMOS operational amplifier while ensuring that the layout satisfies fabrication constraints and closely matches the schematic-level performance.

The complete design flow includes:

* Schematic Design
* Layout Design
* DRC Verification
* LVS Verification
* Parasitic Extraction (PEX)
* Pre-layout Simulation
* Post-layout Simulation
* Performance Comparison

---

## Design Flow

```
Schematic
     │
     ▼
Layout Design
     │
     ▼
DRC Verification
     │
     ▼
LVS Verification
     │
     ▼
PEX Extraction
     │
     ▼
Post-Layout Simulation
     │
     ▼
Performance Comparison
```

---

## Results

### Physical Verification

* ✔ DRC completed successfully (only fabrication-related warnings remain)
* ✔ LVS passed successfully
* ✔ PEX extracted successfully

### Layout

* **Layout Area:** 2025 µm²

---

## Performance Comparison

| Parameter                  | Pre-Layout | Post-Layout |
| -------------------------- | ---------: | ----------: |
| Gain                       |   99.98 dB |   100.05 dB |
| Unity Gain Bandwidth (UGB) |  41.37 MHz |   37.39 MHz |
| Phase Margin               |      68.8° |       68.3° |

---

## Discussion

The post-layout simulation shows excellent agreement with the schematic-level design.

* The gain remains nearly unchanged at approximately **100 dB**, indicating that the amplifier is robust against layout-induced parasitics.
* The **Unity Gain Bandwidth (UGB)** decreases slightly from **41.37 MHz** to **37.39 MHz** due to the additional parasitic resistances and capacitances introduced during layout.
* The **Phase Margin** changes only marginally, confirming that the amplifier maintains good stability after layout implementation.

Overall, the layout preserves the intended electrical performance while satisfying physical verification requirements.

---


---

## Tools Used

* Cadence Virtuoso
* Calibre (DRC/LVS)
* Parasitic Extraction (PEX)
* Spectre Simulator

---

## Reference

For a detailed explanation of the design methodology, layout implementation, verification process, and simulation results, please refer to the accompanying report included in this repository.
