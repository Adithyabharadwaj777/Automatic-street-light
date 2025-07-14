# Automatic Street Light Simulation (Multisim)

This project demonstrates an **Automatic Street Light** system simulated using **NI Multisim**. The system is designed to switch ON a street light automatically when it gets dark and turn it OFF in the presence of daylight, optimizing energy usage.

---

##  Circuit Overview

The circuit uses the following major components:
- **LDR simulation using variable resistors**
- **Operational Amplifier (UA741CP)**
- **NPN Transistor (BC107BP)**
- **LED (as street light)**
- **Resistors for biasing and control**

---

##  Working Principle

The core idea is to use a voltage comparator and an LDR (simulated using resistors or variable resistors in Multisim) to detect ambient light:

- During **daylight**:
  - The LDR (simulated with low resistance) gives higher voltage to the inverting input.
  - The op-amp output remains LOW.
  - Transistor does **not** conduct, so **LED is OFF**.

- During **night**:
  - The LDR (simulated with high resistance) gives lower voltage to the inverting input.
  - The non-inverting input becomes dominant.
  - The op-amp output goes HIGH.
  - Transistor turns ON, **lighting up the LED** (street light turns ON).

---

##  Components Used

| Component         | Quantity |
|------------------|----------|
| UA741 Op-Amp     | 1        |
| BC107 NPN Transistor | 1    |
| LED              | 1        |
| Resistors (various: 200kΩ, 300kΩ, etc.) | Several |
| DC Power Supply (±12V) | 2 |
| Variable Resistors (to simulate LDR) | 2 |

---

##  Software Used

- **NI Multisim 14.x** or later
- Circuit created and simulated successfully

---

##  Features

- Simple analog-based automation system
- Realistic day-night light detection using op-amp
- Easy to extend to real-world applications using actual LDR and relay

---

##  Applications

- Street lighting systems
- Garden and outdoor lights
- Campus or public lighting automation

---

##  How to Use

1. Open the `.ms14` file in Multisim.
2. Run the simulation.
3. Use the **variable resistors** to simulate light intensity (adjust their values).
4. Observe the LED turning ON/OFF automatically based on the resistor settings.

---



##  Author

**Adithya M Bharadwaj**  
Project Date: July 2025  
Simulation Tool: NI Multisim  
