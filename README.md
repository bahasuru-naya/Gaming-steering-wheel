# 🚗 Gaming Steering Wheel (DIY Arduino Project) 🔧

<video src="https://github.com/user-attachments/assets/11464753-b3bd-4498-9799-614f16011214" controls="controls" style="max-width: 100%;"></video>

I recently took on an exciting project to create a **DIY gaming steering wheel with pedals**, all powered by an **Arduino Uno**! This project transforms an Arduino into a plug-and-play USB HID Joystick for your PC.

## 🛠 Features & Innovation

Instead of the commonly used potentiometer for steering input, I decided to use a **rotary encoder** (sourced from an old mouse). 

**Why a Rotary Encoder?**
- **Cleaner Signal:** Digital pulses mean no analog noise or jitter.
- **Better Noise Immunity:** Much less susceptible to electrical interference.
- **Longevity:** Rotary encoders last much longer than potentiometers, which wear out over time—perfect for intense gaming!

## 🔧 Hardware Components
- **Microcontroller:** Arduino Uno (R3)
- **Steering Input:** Rotary Encoder (from an old mouse)
- **Pedals:** Standard pedal assembly integrated into the Arduino logic.
- **Communication:** USB HID via the ATmega16U2 (flashed with UnoJoy).

## 🔌 Circuit Diagram
![image](https://github.com/user-attachments/assets/98db05ff-5cca-4239-8d4b-8fe96c99f39e)

## 💻 Software Implementation

The project relies on efficient interrupt-driven logic and HID emulation:
- **UnoJoy Integration:** Used to make the Arduino appear as a native joystick in Windows/Linux.
- **Interrupt System:** Uses pins **2 and 3** to handle high-speed inputs from the rotary encoder without missing steps.
- **Microcontroller Reprogramming:** To enable HID mode, I reprogrammed the Arduino's 16U2 chip using **FLIP software**.




