# STM32F103C6 - 2 Button & 3 LED Control Project

This is a basic embedded systems (my first)project using the STM32F103C6 microcontroller to control three LEDs with two buttons.

## 🧠 Project Description

In this project:
- Two buttons are used to control the sequence and direction of three LEDs.
- The LEDs (Red → Blue → Green) light up one at a time in a specific order.
- Pressing the **Set** button reverses the LED sequence direction (forward/backward).
- Pressing the **LED** button switches to the next LED in the current direction.

## 🔧 Hardware Components

- STM32F103C6T6 ("Blue Pill")
- 2x Push Buttons
- 3x LEDs (Red, Blue, Green)
- 330 Ohm resistors for LEDs
- Breadboard and jumper wires

## 🧷 Pin Configuration

| Component     | MCU Pin         |
|---------------|------------------|
| Set Button    | PA0              |
| LED Button    | PA1              |
| Red LED       | PB0              |
| Blue LED      | PB1              |
| Green LED     | PB2              |

> Note: The buttons are configured with `GPIO_PULLDOWN`.

## ⚙️ Software Information

- Developed using **STM32CubeIDE**
- Utilizes **HAL (Hardware Abstraction Layer)** drivers
- `HAL_GPIO_ReadPin()` is used to read button states
- `HAL_GPIO_WritePin()` is used to control LED states
- `isStraight` boolean variable determines the direction of the LED sequence
- A basic `HAL_Delay()` is used to debounce the buttons

## 📷 Visuals
![schematic](https://github.com/user-attachments/assets/92b37128-6a4b-479d-ba3a-78066c6a18e7)

## 📄 License

MIT License  
This project is free to use, modify, and share for learning and development purposes.

## README preparing 
I used ChatGPT to help me write this README file and I'm trying learn that how to write one. 
