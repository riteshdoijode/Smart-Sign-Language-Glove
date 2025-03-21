# Smart Glove Project

This Arduino-based **Smart Glove** is designed to interact with sensors, buttons, and an OLED display. The glove can detect hand movements, recognize gestures, and display relevant information on an OLED screen.

## Features

- **Gesture Recognition:** Uses sensor thresholds to interpret hand movements.
- **OLED Display:** Outputs text or graphics using an **Adafruit SSD1306** OLED module.
- **Button Input:** Captures button presses with **debouncing** logic to avoid false triggers.
- **Audio Output (PCM Library):** Potentially enables sound feedback.
- **Efficient Memory Use:** Stores predefined graphical data in **PROGMEM** for display.

## Hardware Requirements

- **Arduino Board** (e.g., Uno, Nano)
- **Adafruit SSD1306 OLED Display**
- **Push Button** (Connected to pin 12)
- **Sensors** (Possible flex sensors or IMU for gesture detection)
- **Wires & Resistors** (for button and sensor connections)

## Software Requirements

Ensure you have the following Arduino libraries installed:

```cpp
#include <PCM.h>
#include <Wire.h>
#include <Adafruit_GFX.h>
#include <Adafruit_SSD1306.h>
```

To install these:
1. Open the **Arduino IDE**.
2. Go to **Sketch** → **Include Library** → **Manage Libraries**.
3. Search for `Adafruit GFX` and `Adafruit SSD1306`, then install them.

## Wiring Guide

- **Button Pin:** Connect to Arduino **Pin 12**.
- **OLED Display:** Connect **SDA** and **SCL** to Arduino's **I2C** pins.
- **Sensors:** Attach to analog/digital pins as per your setup.

## Usage

1. **Upload the Code:**  
   - Open `glove.ino` in Arduino IDE.  
   - Select the correct **Board & Port**.  
   - Click **Upload**.  

2. **Wear the Glove:**  
   - Ensure the sensors are properly positioned.  
   - Press the button or move fingers to see OLED responses.  

3. **Observe the Display & Output:**  
   - The OLED screen will show relevant text/images.  
   - Depending on the setup, audio feedback may also be provided.  

## Future Improvements

- Add **Bluetooth or Wi-Fi** support for wireless communication.
- Implement **Machine Learning** to improve gesture recognition.
- Expand to **assistive technology** applications for speech-impaired users.

## License

This project is open-source under the MIT License.

---

👨‍💻 Developed by Ritesh Doijode.
```
