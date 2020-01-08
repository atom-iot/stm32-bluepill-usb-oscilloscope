# stm32-bluepill-usb-oscilloscope

A simple oscilloscope using the STM32 blue pill board

It keeps sending channel 3 then channel 4, as a 2500 sample/chunk (with a total of 20 chuncks sent)

Each sample is 2 bytes, so each chunk size must be 5000 bytes

And each chunk is sent every 50 ms, and each new second, it replaces one of the nearby samples with "0xFFFF" to notify the host of the new second.


