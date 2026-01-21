# STM32F401 LED and Button Interfacing (Polling & Interrupt)

This project demonstrates **LED and push button interfacing** using the **STM32F401RBT6 (Nucleo-64)** board.
Both **Polling** and **Interrupt (EXTI)** methods are implemented using **on-board components only**.

---

## 🧠 Objective
- To control an LED using a push button
- To understand the difference between **Polling** and **Interrupt** methods
- To implement **external interrupt (EXTI)** with software debouncing

---

## 🧩 Hardware Used
- **Board:** STM32F401RBT6 (Nucleo-64)
- **On-board LED:** PA5 (LD2)
- **User Button:** PC13 (B1)
- ❌ No external LED or breadboard used

---

## 🧰 Software Used
- STM32CubeIDE
- STM32 HAL Library
- STM32CubeMX (.ioc configuration)

---

## ⚙️ Pin Configuration
| Component | Pin | Mode |
|--------|-----|------|
| LED | PA5 | GPIO Output |
| Button | PC13 | GPIO Input with EXTI (Falling Edge) |

---

## 🔁 Working Description

### 🔹 Polling Method
- Microcontroller continuously checks the button status
- LED turns **ON while button is pressed**
- LED turns **OFF when button is released**

### 🔹 Interrupt Method
- Button press generates an **external interrupt (EXTI)**
- LED toggles **once per button press**
- Software debouncing is implemented to avoid multiple triggers

---

## 📌 Key Learning
- Difference between **level-based (polling)** and **event-based (interrupt)** handling
- Importance of **debouncing** in mechanical switches
- Proper STM32 project structure and interrupt handling

---

