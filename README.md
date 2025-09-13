EventBoard - RTC-Driven Message Display System
📌 Overview

The EventBoard is an embedded system project designed to display predefined messages on an LCD at specific times using the RTC (Real-Time Clock) of the LPC2148 microcontroller.

It includes:

Automated message scheduling

Password-protected admin mode

Real-time temperature display (using LM35 sensor)

Visual indicators via LEDs

Secure time and message management

⚙️ Features

⏰ RTC-based scheduling – Messages are displayed at specific times.

🔐 Admin Mode – Access secured with a switch and password-protected keypad.

📝 Editable Messages – Select which messages are active for the day.

🌡️ Temperature Monitoring – Displays room temperature when idle.

💡 LED Indicators – Green = active schedule, Red = idle display.

🔊 Buzzer Support – For event alerts.

🛠️ Requirements
Hardware

LPC2148 Microcontroller

16x2 LCD

Keypad

LEDs (Red/Green)

LM35 Temperature Sensor

Buzzer

Software

Embedded C

Keil uVision (C Compiler)

Flash Magic (Programming Tool)

🚀 How It Works

Normal Mode:

Displays scheduled messages on LCD at the set time.

If no message is scheduled, shows RTC time and room temperature.

Admin Mode (Switch + Password):

Modify RTC time.

Enable/disable messages for the day.

Indicators:

Green LED → Scheduled message active.

Red LED → Idle (showing clock/temperature).

📋 Example Messages

The system comes with 10 predefined messages (all enabled by default):

07:45 → Good Morning! Classes Start Soon

13:45 → C Programming Session in Class Room 2

10:15 → C Module Theory Exam – Lab1 (4th Floor)

12:45 → Lunch Break from 1PM – 2PM

17:45 → End of Day – See You Tomorrow!

(and more… up to 10 messages)

🖼️ Block Diagram

(Add block diagram image here if available, e.g., ![Block Diagram](images/block_diagram.png))

✅ Ready to flash on LPC2148 and demonstrate automated event scheduling with real-time updates.

Would you like me to also add a “Project Setup & Usage” section (steps to compile in Keil, burn with Flash Magic, run on LPC2148), or keep this README lightweight?

You said:
please give me the other one ,i think this is not good
ChatGPT said:

Got it 👍
Let me create a different style of README – shorter, cleaner, and more GitHub-friendly (something that looks nice at first glance, without too many technical paragraphs).

⏰ EventBoard – RTC Driven Message Display

A simple embedded system project using the LPC2148 microcontroller to display scheduled messages on an LCD with real-time updates.

✨ Highlights

📢 Displays scheduled messages automatically

🔐 Secure Admin Mode (switch + keypad + password)

🕒 RTC based control for accuracy

🌡️ Shows temperature using LM35 sensor when idle

💡 LED indicators:

Green → Active schedule

Red → Idle mode

🛠 Hardware

LPC2148

16x2 LCD

Keypad

LEDs (Red/Green)

LM35 Temperature Sensor

Buzzer

💻 Software

Embedded C (Keil µVision)

Flash Magic (programming tool)

🚀 Quick Workflow

System starts in Normal Mode.

If time matches a scheduled message → show it on LCD.

Otherwise → show RTC time + temperature.

Enter Admin Mode using switch + password.

Change RTC time.

Enable/disable daily messages.

📋 Default Messages

Some predefined schedules:

07:45 → Good Morning! Classes Start Soon

10:15 → C Module Exam (Lab1 – 4th Floor)

12:45 → Lunch Break (1–2 PM)

17:45 → End of Day – See You Tomorrow!

✅ Compact, secure, and real-time message display system.
