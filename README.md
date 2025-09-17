# Solar-Powered Home Automation with Load Management

## Project Overview
This project demonstrates a **solar-powered home automation system** that controls lights, fans, and small appliances based on the availability of solar energy. It uses **Arduino** (or Raspberry Pi), relays, and sensors to automatically manage loads, prioritize essential devices, and ensure efficient use of renewable energy.  

---

## Features
- **Solar Power Integration:** Loads are powered primarily by solar energy.  
- **Automatic Load Management:** Prioritizes essential appliances when solar power is limited.  
- **Relay-Based Switching:** Automatic on/off switching of devices based on sensor readings.  
- **Manual Override:** Users can manually control devices if needed.  
- **Affordable & Easy:** Uses widely available components for practical implementation.  

---

## Modules Covered
| Module | Application in Project |
|--------|----------------------|
| Basic Electrical Engineering | Circuit design, wiring, and basic electrical components |
| Renewable Energy Sources | Solar panel integration as the primary energy source |
| Electric Drives & Control | Control of DC/AC motors (fans, pumps) |
| Special Motors | Small appliances motor control |
| Distributed Generation | Solar energy as distributed energy |
| Power System Protection & Switchgear | Fuses, relays for safe operation |
| Creative & Management | Designing system layout and implementing the prototype |

---

This repo includes a minimal sketch for the **solar load controller** and a **CI workflow** that compiles it using Arduino CLI.

## Install Arduino CLI
```bash
curl -fsSL https://raw.githubusercontent.com/arduino/arduino-cli/master/install.sh | sh
arduino-cli version
```

## Cores & board (UNO example)
```bash
arduino-cli core update-index
arduino-cli core install arduino:avr
```

## Compile
```bash
arduino-cli compile --fqbn arduino:avr:uno arduino/sketches/solar_controller
```

## Upload (set your serial port)
```bash
arduino-cli upload -p /dev/ttyACM0 --fqbn arduino:avr:uno arduino/sketches/solar_controller
```

> If you use a different board (e.g., ESP32), install the appropriate core and update the **FQBN** in commands and CI.

## Components Required
- Arduino Uno (or Raspberry Pi)  
- Solar panel (5V–12V)  
- Relay module (for AC load switching)  
- Light sensor / voltage sensor  
- DC/AC fan, LED bulbs, or small appliances  
- Jumper wires, breadboard, resistors, fuses  

---

## Contact  
For questions, collaboration, or feedback, please contact:  
**Sammeta Dinesh Kumar** — [sammetadineshkumar@gmail.com]
- 🌐 [Portfolio](https://dineshkumarsammeta.github.io/)
- 🔗 [LinkedIn](https://www.linkedin.com/in/dineshsammeta)   

## Circuit Diagram
![Circuit Diagram](Circuit_Diagram.png)  
*Include an image of your wiring diagram here.*
