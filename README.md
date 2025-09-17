Here’s a polished **project description + proposal** you can drop directly into your repo’s `README.md` file for the **Microwatt + Crypto Acceleration SoC** idea:

---

# Microwatt + Crypto Acceleration SoC

**Secure Edge Computing with Open-Source POWER + Hardware Crypto**

## Overview

This project extends the **Microwatt POWER CPU core** with a dedicated **cryptographic accelerator** to enable secure and efficient edge computing. By integrating hardware implementations of **AES (Advanced Encryption Standard)**, **SHA-2 hashing**, and optional **Post-Quantum Cryptography (PQC) primitives**, this SoC demonstrates how open-source CPUs can be enhanced for **trustworthy IoT and communication applications**.

Microwatt acts as the control and application processor, while the custom accelerator performs computationally expensive crypto operations at hardware speed. This hybrid design reduces CPU load, improves throughput, and enables **secure boot, data encryption, and authentication** in resource-constrained environments.

---

## Motivation

Security is a cornerstone of the open computing era. As open-source hardware adoption grows, the need for **transparent and reproducible crypto solutions** becomes essential. While Microwatt provides a general-purpose POWER ISA CPU core, many security workloads (key exchange, hashing, encryption) benefit from dedicated hardware.

This project demonstrates that **open hardware can be both innovative and secure** by pairing Microwatt with a modular, open-source cryptographic accelerator.

---

## Project Objectives

* Extend Microwatt with a **crypto acceleration block** supporting:

  * AES-128/256 (block cipher for data encryption)
  * SHA-256 (hashing for authentication and signatures)
  * Optional PQC algorithm (e.g., Kyber KEM or Dilithium)
* Provide **memory-mapped I/O (MMIO) interface** for CPU ↔ Crypto core communication.
* Demonstrate **secure boot flow**: Microwatt verifies firmware integrity using hardware SHA.
* Support **real-world IoT use cases**, such as sensor data encryption before transmission.
* Ensure **open-source reproducibility** with documented toolchains, flows, and testbenches.

---

## Key Technologies & Tools

* **Microwatt CPU Core** ([OpenPOWER Foundation](https://git.openpower.foundation/cores/microwatt))
* **OpenPOWER ISA** for application-level software development
* **Crypto Accelerator RTL** (AES, SHA, PQC modules coded in Verilog/VHDL with AI-assisted generation)
* **FPGA/ASIC Flow Tools:**

  * GHDL, Yosys, Verilator, NextPNR (simulation/synthesis)
  * OpenLane / ChipIgnite flow for SKY130 implementation
* **Software Toolchains:** GCC for POWER, GDB, crypto test libraries

---

## Expected Deliverables

* RTL implementation of AES/SHA/PQC accelerator modules
* Testbenches for unit-level and system-level verification
* Constraints and timing files for STA + SDF simulation
* Full SoC integration with Microwatt core
* Demo applications:

  * Secure boot verification
  * Sensor data encryption & decryption pipeline
* Documentation of AI-assisted design process (prompts + GPT logs)
* Open-source license (Apache-2.0 or MIT)

---

## Impact & Value

* **Practical & Relevant:** Demonstrates secure open-source SoC design for IoT/edge computing.
* **Innovative:** Integrates post-quantum crypto in a lightweight, reproducible flow.
* **Reproducible:** Fully open toolchain and SKY130 compatibility.
* **Community Value:** Serves as a reference design for other open hardware developers exploring CPU + accelerator architectures.

---

## Program Timeline Alignment

* **Proposal Submission (Sep 22, 2025):** Initial README with design description (this file).
* **Final Submission (Nov 3, 2025):** Complete SoC RTL, testbenches, documentation, and demo.
* **Deliverables:** Final GitHub repo including source code, simulation results, build flow, and video demo.

---

## License

This project is licensed under the **Apache 2.0 License** – ensuring open collaboration and reproducibility.

---

## Resources

* [Microwatt Core](https://git.openpower.foundation/cores/microwatt)
* [OpenPOWER Foundation](https://openpowerfoundation.org/)
* [ChipFoundry](https://chipfoundry.io/start-a-project)
* [OpenLane / ChipIgnite Flow](https://github.com/The-OpenROAD-Project/OpenLane)



 **Theme Fit:**
"Microwatt for the open computing era" – This project showcases how Microwatt can form the foundation of a secure, open, and extensible SoC platform by integrating hardware cryptography into the open-source computing stack.

