# TinyCircuits Graphics Buffer Library

This Arduino library is intended for use with TinyCircuits' **[0.42" OLED Wireling](https://tinycircuits.com/collections/wireling-displays-leds/products/0-42-oled-screen-wireling)**, **[0.69" OLED Wireling](https://tinycircuits.com/collections/wireling-displays-leds/products/0-69-oled-screen-wireling)**, and **[0.96" OLED Wireling](https://tinycircuits.com/collections/wireling-displays-leds/products/0-96-oled-screen-wireling)**. 

*Support this library by buying products from **[TinyCircuits](https://tinycircuits.com/)***


## Graphics Buffer Class Basics

After using the constructor *GraphicsBuffer(const uint16_t widthInit, const uint16_t heightInit, const uint8_t bitsPerPixelInit)* to create a Graphics Buffer object using the width, height, and BPP, you can use any of the following functions to add a graphic or text element to a buffer to send and display on a screen. To display the buffer on the screen, you will need to use the **[TinierScreen library](https://github.com/TinyCircuits/TinyCircuits-TinierScreen-Lib)** that the Graphics Buffer library example depends upon.

* **void writePixel(uint16_t color)** 
* **void setX(uint8_t, uint8_t)**
* **void setY(uint8_t, uint8_t)**
* **void goTo(uint8_t x, uint8_t y)**
* **void drawPixel(uint8_t, uint8_t, uint16_t)**
* **void clear()**
* **void clearWindow(uint8_t x, uint8_t y, uint8_t w, uint8_t h)**
* **void drawLine(int16_t x0, int16_t y0, int16_t x1, int16_t y1, uint16_t color)**
* **void drawCircle(int16_t x0, int16_t y0, int16_t radius, uint16_t color)**

## Graphics Buffer Class Font

* **void setFont(const FONT_INFO&)**
* **uint8_t getFontHeight(const FONT_INFO&)**
* **uint8_t getFontHeight(void)**
* **uint8_t getPrintWidth(char *)**
* **void setCursor(int, int)**
* **void fontColor(uint16_t, uint16_t)**
* **virtual size_t write(uint8_t)**
* **uint8_t* getBuffer()**
* **uint16_t getBufferSize()**
