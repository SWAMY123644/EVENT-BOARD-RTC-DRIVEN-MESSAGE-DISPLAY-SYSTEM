# ⏰ EventBoard – RTC-Based Automated Message Display

## 📌 Overview
**EventBoard** is an embedded system built on the **LPC2148 ARM7 microcontroller**.  
Its purpose is to automatically show scheduled messages on a **16x2 LCD** using the **Real-Time Clock (RTC)**.

The system also includes:  
- Secure **Admin Mode** with keypad + password access  
- Editing of **RTC time** and enabling/disabling messages  
- **Temperature monitoring** via LM35 sensor  

---
## ⚙ Hardware Components
- LPC2148 Microcontroller  
- 16x2 LCD Module  
- 4x4 Keypad  
- Status LEDs (**Green = Active**, **Red = Idle**)  
- LM35 Temperature Sensor  
- Buzzer  

---

## 💻 Software Tools
- Embedded C  
- **Keil µVision** (C Compiler & IDE)  
- **Flash Magic** (for programming LPC2148)  

---

## 🔄 Operating Modes

### Normal Mode
- LCD continuously shows RTC time  
- If the current time matches a scheduled event → message scrolls on LCD & **Green LED** lights up  
- If no message is scheduled → LCD displays time + room temperature & **Red LED** lights up  

### Admin Mode
- Entered via **external switch interrupt**  
- Secured with **password-protected keypad input**  
- Provides options to:  
  - Edit RTC date/time  
  - Configure and activate/deactivate scheduled messages  

---

## 📂 Project Structure

| File / Folder                     | Description |
|----------------------------------|------------|
| `Event_Board_Main.c`              | Main entry file – integrates LCD, keypad, RTC, ADC, and settings |
| `lcd.c / lcd.h`                   | LCD driver – initialization, command/data functions, string/number display |
| `kpm.c / kpm.h`                   | Keypad driver – scanning rows/columns, key detection, numeric/password input |
| `adc.c / adc.h`                   | ADC driver – reads LM35 sensor values and converts to digital |
| `rtc.c / rtc.h`                   | RTC driver – initialization, set/get current date/time, display on LCD |
| `settings.c / settings.h`         | Settings manager – update RTC and stored message configurations |
| `delay.c / delay.h`               | Delay utilities – software-based ms/sec delays for timing |
| `pin_connect_block.c / pin_connect_block.h` | Pin configuration – sets pin functions for peripherals |
| `defines.h / types.h / interrupts_defines.h` | Shared headers – macros, typedefs, and interrupt definitions |

---

## 🚀 Key Features
- ⏰ RTC-based scheduled message display  
- 📜 Scrolling messages on LCD  
- 🔑 Secure Admin Mode with password protection  
- 🌡 Real-time temperature sensing (LM35)  
- 🔴🟢 LED-based status indication  

---

## 🎯 Use Cases
- 🏫 Smart school/college notice boards  
- 🏢 Office reminders and event notifications  
- 🔬 Lab automation and schedule displays  
- 🏠 Home information displays
