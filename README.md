# STM32_GIF_decode

This a project using stm32 to decode gif files from sd card, and display the gif image on the screen. The project uses DMA2D, so CPU only needs to decompress the Lzw data from gif and store in display memory. As the project ported Craig A. Lindley's gif library, you have to customize your own display and file operation callback functions. Those callback function which you need to set up is on the GifDecoder_lmpl.h file.

## Demo

https://www.youtube.com/watch?v=ZMFxSXhdmFI


## Todo

* Add FreeRTOS to the project.
* improve efficiency, especially for those high rate gif files.