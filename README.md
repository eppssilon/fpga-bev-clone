# FPGA-Based Bird’s Eye View Image Processing for ADAS

**Internship Project – Capgemini Engineering Casablanca, Summer 2025**
**Authors / Contributors:** Adam El Meziane, Oumaima El Atrache
**Mentors:** ECH-CHARRAQ Saad, ZIDANI Saad, SMAALI Abderrahmane

---

## Project Overview

This project implements **Bird’s Eye View (BEV) image processing on an FPGA** for Advanced Driver Assistance Systems (ADAS). It focuses on real-time sensor fusion, memory management, and camera-to-display processing using **SystemVerilog** on the **RZ easyFPGA A2.2 (Cyclone IV) board**.

The goal was to develop and verify IP modules for image capture, SDRAM handling, and VGA display while exploring **UVM-based verification methodologies**.

---

## Tools & Environment

* FPGA Design & Synthesis: **Quartus**
* Simulation & Verification: **ModelSim, MATLAB/Simulink**
* Auxiliary Scripts: **Python**

---

## Repo Structure

```
fpga-bev/
│
├─ src/                # SystemVerilog source files (IP modules, top-level design)
├─ tb/                 # Testbenches
├─ scripts/            # Python scripts for memory and image processing
├─ assets/             # Sample images, captured outputs, and test data
├─ output_files/       # Compilation/synthesis outputs and reports
├─ .qsys_edit/         # Qsys/Platform Designer intermediate files
├─ db/                 # Quartus database files
├─ greybox_tmp/        # Temporary compilation files
├─ incremental_db/     # Incremental compilation files
├─ led_debug_test.sv   # Example LED debug module
├─ pfa_sensor_fusion.* # Quartus project files
├─ pll_133Mhz.*        # PLL IP implementation
├─ sdram_*.*           # SDRAM controller and FSM definitions
```

---

## Key Features / Modules

* **Sensor Fusion IP Modules**: Combine multiple camera inputs for BEV rendering.
* **SDRAM Controller**: Efficient memory initialization, read/write FSMs, and high-speed interface.
* **Camera Capture**: Multi-camera capture system for input images (OV7670).
* **VGA Display**: Real-time output to VGA, including frame reader and test patterns.
* **Verification**: Testbenches for SDRAM and camera modules, supporting UVM-based validation.

---

## Notes

* Project currently focuses on FPGA implementation and simulation; hardware setup instructions can be added later.
* Contributors handled all source design, simulation, and system integration collaboratively.

---

## Acknowledgements

Special thanks to **@ECH-CHARRAQ Saad**, **@ZIDANI Saad**, and **@SMAALI Abderrahmane** for their mentorship, and **@EL ATRACHE Oumaima** for being an incredible partner-in-crime throughout the project
