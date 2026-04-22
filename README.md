#  Nokia 5110 LCD (PCD8544) Display Project

This project demonstrates how to use a Nokia 5110 LCD display with an Arduino to show bitmap images and graphics.

---

## Hardware Required

- Arduino Uno / Nano / Mega  
- Nokia 5110 LCD (PCD8544)  
- Jumper wires  
- 3.3V power source (important!)

---

##  Wiring (Connections)

| LCD Pin | Arduino Pin |
|--------|------------|
| RST    | 12         |
| CE/SCE | 11         |
| DC     | 10         |
| DIN    | 9          |
| CLK    | 8          |
| VCC    | 3.3V       |
| GND    | GND        |

---

##  Features

- Display bitmap images on Nokia 5110 LCD  
- Custom graphics using byte arrays  
- Low-level control using shift registers  
- Lightweight and fast Arduino code  

---

##  How It Works

The display is controlled using SPI-like communication:
- `LcdWrite()` sends commands/data to the display
- `LcdBitmap()` draws images stored in byte arrays
- Pixel data is stored in PROGMEM to save RAM

---

## Example Bitmap

The project includes a sample bitmap image:

```cpp
char bmp1[] = {
  // image data (generated using LCD bitmap converter)
};
