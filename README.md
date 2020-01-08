# stm32-bluepill-usb-oscilloscope

A simple oscilloscope using the STM32 blue pill board

It keeps sending the first channel 3 then channel 4, as a 2500 sample/chunk

Each sample is 2 bytes, so each chunk size must be 5000 bytes

And each chunk is sent every 50 ms, and every new second, it adds "0xFFFF" in the samples to notify the host of the new second.


