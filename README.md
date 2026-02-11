# Embedded Energy Measurement Recalibrator ⚡🛠️

This project is a **recalibrator for an energy measurement system**. It was created during my bachelor’s days, so please go easy on the design! 😅  

---

## Hardware 🖥️

- **Freescale 32-bit microcontroller** (a bit old, but reliable)  
- **Nokia 1100 LCD** for simple display output  
- **XBee module** for mesh network communication  
- **Numeric keypad with arrows** for menu navigation  

---

## Software Architecture 💻

The software is designed around a **main event loop** combined with **interrupt-driven handlers**:

- The **main loop** handles general tasks such as menu updates, sensor readings, and network communication.  
- **Interrupt routines** respond to time-critical events like button presses, XBee messages, and peripheral readings.  
- This architecture ensures that **time-sensitive operations are handled immediately**, while the main loop manages the overall workflow efficiently.  

> Think of it as a combination of **polling + reactive event handling** – common in embedded systems. ⚡

---

## Features ✨

- Recalibrates energy measurement devices automatically  
- Displays menu and status on the Nokia LCD  
- Communicates with other devices via XBee mesh network  
- Uses a simple, robust embedded software architecture  

---

## Note 📝

- This is an **older bachelor project**, so don’t expect cutting-edge hardware or software practices.  
