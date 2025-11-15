
## 😴 Drowsy Driver Detection System: 8051 Microcontroller Implementation

This project outlines a **safety technology** designed to monitor a driver's alertness level and detect signs of fatigue or sleepiness while driving. Its core goal is to **prevent accidents** caused by a tired or inattentive driver by issuing warnings or taking corrective actions.

---

### 🎯 System Operation and Logic

The system uses an **eye blink sensor** to monitor the driver's face and eyes. The logic for detection and response is as follows:

| Driver State | Sensor Logic | Motor/Vehicle | Buzzer | Screen Message |
| :--- | :--- | :--- | :--- | :--- |
| **Drowsy/Sleeping** | **Logic Zero (0)** | **Motors Off** | **Counts High/ON** | "Driver is Sleeping" |
| **Alert/Not Sleeping** | **Logic One (1)** | **Keeps Running/ON** | **OFF State** | "Driver NOT Sleeping" |

---

### ⚙️ Hardware and Software Tools

#### 8051 Microcontroller (Core Component)

The system is built around the **8051 microcontroller**, an 8-bit MCU known for its simplicity and versatility.

* **CPU:** Handles arithmetic and logical operations, and controls the flow of instructions.
* **Memory:** Includes **4KB ROM** for program storage and **128 bytes RAM** for data storage and temporary variables.
* **I/O Ports:** Four **8-bit bidirectional ports (P0 to P3)** are used for interfacing with external devices, such as the eye blink sensor and the buzzer/motor control circuits.
* **Timers/Counters:** Features two 16-bit timers (Timer 0 and Timer 1) for timing operations and event counting.
* **Communication:** A built-in UART allows for serial communication.
* **Interrupts:** Five interrupt sources are available for handling asynchronous events.
* **Clock:** Typically operates using a **12 MHz crystal oscillator**.

#### Software and Simulation

The project utilizes the following industry-standard tools for development and testing:

* **Keil µVision:** The IDE used for writing, compiling, and debugging the C or assembly code for the 8051 microcontroller.
* **Proteus:** The simulation software used to design the electronic circuit and simulate the behavior of the 8051, sensor, motor, and buzzer in a real-time environment.
