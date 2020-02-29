# Download Firmware

&nbsp;

## Via DFU Mode

- How to access DFU mode.

  - If the circuit board is not connected to the computer —— press the "USER" button of the Lora node before inserting it into any USB port of the computer (press the “USER"  key all the time before inserting, and release it after connecting to the USB port)
  - If the board had connected to the computer —— Keep the “USER” button pressed → Press the "RST" button → Release the "RST" button → Release the "USER" button.

- Download firmware.

  If enter DFU mode successfully (with the driver is installed correctly), you can see the device named "STM32 BOOTLOADER" in the device manager. In the STM32CubeProg software, select USB and click “Connect” to read the chip information.

  ![](img/download_firmware/03.png)

  Open a .hex/.bin file and click the "Download" icon.

  ![](img/download_firmware/04.png)

  ***The advantage of using the DFU mode is that you can easily find a Micro USB cable. But the disadvantage is that there is no way to simulate online.***

## Via ST-LINK

- How to connect to ST-LINK.

  Connect the ST-LINK to the LoRa Node correctly,please refer to this picture.

  ![](img/download_firmware/01.png)

  ```Tip:: ST-LINK can provide power to target device! If the LoRa Node is connected to the computer via the Micro USB interface, the ST-LINK 3.3V CAN NOT be connected to the VDD! Doing so may damage  the development board!
  
  ```

- Download firmware.

  After connecting ST-LINK correctly,click on this icon.

![](img/download_firmware/02.png)

***The advantage of using the ST-LINK method is that it can be single-stepped debugging with the STM32CubeIDE , but the disadvantage is that the ST-LINK debugger tool is required.***