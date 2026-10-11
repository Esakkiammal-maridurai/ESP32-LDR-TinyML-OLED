# Live Sensor + TinyML on ESP32

## Project Description

This project demonstrates how to interface an **LDR (Light Dependent Resistor)** sensor with an ESP32 and use a **TensorFlow Lite for Microcontrollers (TFLite Micro)** model to classify real-time light readings as **Dark, Normal, or Bright**.

The real-time LDR sensor reading is given as input to the on-device TinyML model, and the predicted class is displayed on an **OLED display**.

## Objective

- Interface an LDR sensor with ESP32.
- Read real-time light intensity values.
- Use TensorFlow Lite for Microcontrollers.
- Classify the light level as Dark, Normal, or Bright.
- Display the sensor reading and predicted class on an OLED.

## Components Required

- ESP32 Development Board
- LDR Sensor
- SSD1306 OLED Display
- USB Cable
- Arduino IDE
- TensorFlow Lite for Microcontrollers library
- Trained `.tflite` model
- Jumper Wires

## Working

```text
LDR Sensor
     ↓
ESP32
     ↓
Read Real-Time Light Value
     ↓
TFLite Micro Model
     ↓
Classify Light Level
     ↓
Dark / Normal / Bright
     ↓
Display Result on OLED
```

## Example

The LDR continuously measures the light intensity.

```text
LDR Reading: 28
```

The TensorFlow Lite Micro model processes the reading and predicts the light level.

```text
Predicted Class: Normal
```

The result is displayed on the OLED.

```text
Light: 28
Status: Normal
```

## Technologies Used

- ESP32
- LDR Sensor
- SSD1306 OLED
- Arduino IDE
- C/C++
- TensorFlow Lite
- TensorFlow Lite for Microcontrollers (TFLite Micro)
- TinyML

## Expected Output

The OLED displays the real-time LDR reading and the predicted light classification.

```text
LDR: 28
Status: Normal
```

The classification changes according to the real-time light intensity.

```text
Dark
Normal
Bright
```

## Result

The LDR sensor was successfully interfaced with the ESP32, and real-time light readings were classified as **Dark, Normal, or Bright** using a TensorFlow Lite Micro model. The predicted result was successfully displayed on the OLED.
