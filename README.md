# Schneider Altivar VFD I/O Configuration and Safety Reference

This repository serves as a technical reference detailing the essential Input/Output (I/O) configuration and safety setup for Schneider Electric Altivar Variable Frequency Drives (VFDs), namely the **ATV212, ATV312, and ATV320**.

This work was conducted as part of an industrial automation internship, focusing on direct VFD commissioning and signal integration.

## 🛡️ Note on Confidentiality

This project strictly adheres to confidentiality clauses. All documentation and settings provided here are **abstracted and de-sensitized** from the actual application data. They serve only as a **template and methodology demonstration** of best practices in industrial VFD commissioning.

## ⚙️ Core Technical Focus

The repository demonstrates competence in the following areas of VFD integration:

### 1. 4-20mA Analog Control Reference

Details the configuration methodology for the VFD's Analog Input (AI) terminals.

* **Objective:** To receive a standard industrial **4-20mA signal** (e.g., from a flow or pressure transmitter) and use it as the direct speed/frequency reference for the motor.
* **Competence Demonstrated:** Understanding of **signal sourcing**, **filtering**, and **internal parameter scaling** (mapping 4mA to 0% speed and 20mA to 100% speed) within the Altivar VFD environment.

### 2. Digital I/O and Safety Configuration

Documents the process of mapping digital inputs and outputs to specific control functions.

* **Digital Input Configuration:** Assignment of terminals (LIx) for fundamental control functions (Start/Stop, Local/Remote control switching).
* **Safety Circuit Integration:** Implementation of the control logic to manage safety signals. This ensures that a critical signal (e.g., Emergency Stop) is mapped to a VFD terminal to trigger an immediate, pre-defined safe stop sequence, ensuring compliance with basic safety requirements.
* **Status Outputs:** Configuration of relay outputs (Ryx) to provide essential drive status feedback (e.g., "VFD Running," "VFD Fault") to the wider control system.

## 📂 Repository Contents

| Directory/File | Description |
| :--- | :--- |
| **`/manuals`** | Official user manuals and programming guides for the ATV212, ATV312, and ATV320 (General documentation only). |
| **`/states`** | Includes the proprietary VFD configuration files created during the project, demonstrating the use of Schneider's SoMove software. |

---

## 🛠️ Software Used

* Schneider Electric SoMove (or equivalent VFD commissioning software).
* *Reference material may be used with any control system (PLC) capable of providing 4-20mA and digital signals.*
