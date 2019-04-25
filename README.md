# RTC-Watch-HAL
Using RTC with LSE at STM32F4Discovery board (stm32f407vg). 
Output in display oled 0.96" 126x64 (ssd1306) by I2C interface. Timer 6 interrupt used for update lcd screen. 
On stm32f4discovery board you need to set X3 crystal (32768 Hz) and C16 and C22 (6.8pF). 
If you havn't X3 crystal you should edit the code and set LSI using in RCC section. 

For well working you need:
- STM32F4Discovery board (any modification) with installed X3 crystal and C12, C22 capasitors.
- 0.96" oled display 128x64 pixels.
Also on your board must fitted X3 crystal (32.768KHz) and two ceramic capacitor 6.8pF. (Not installed by factory).
Create a template by STM32CubeMX. STM32CubeMX version is 5.0.1 used. Driver version is STM32Cube FW_F4_V1.23.0. Open watch.ioc file in STM32CubeMX and generate template.
Connect display to board. Replace files in your project. Build project.
Enjoy =)
