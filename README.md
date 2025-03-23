# ax1600i-usb-dump

This is a wireshark USB filtered capture of a Corsair AX1600i PSU while running iCue.

It's about 30 seconds long and I performed the following tasks.

* Plug in the USB cable.
* iCue (already running) grabbing the following data (during the whole capture):
  * Fan (RPM)
  * Temp (C)
  * Power in (W)
  * Power out (W)
  * Efficiency (%)
  * 12V Voltage (V)
  * 5V Voltage (V)
  * 3.3V Voltage (V)
  * 12V Current (A)
  * 5V Current (A)
  * 3.3V Current (A)
  * 12V Power (W)
  * 5V Power (W)
  * 3.3V Power (W)
* I change the fan preset to a profile called "high" (fixed 100%)
* Change the preset to "low" (fixed 40%)
* Change the preset back to default (fan turns off again)

I'm not sure if the fan curves from iCue are managed by iCue itself or if it stores the curve in the PSU. But I can do another capture in the future to check this.

I hope this is enough for someone to write a driver for Linux.


