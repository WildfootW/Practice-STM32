# STM32 & ARM Cortex-M Toolchain
[TOC]
###### tags: `Embedded` `ARM` `STM32`

# Resources / References
* [Hands-On RTOS with Microcontrollers, published by Packt](https://github.com/PacktPublishing/Hands-On-RTOS-with-Microcontrollers)

# Software
## STM32
* [STM32F4 Discovery board Tutorial (CubeMX with Keil 5)](https://www.youtube.com/playlist?list=PLfExI9i0v1sn_lQjCFJHrDSpvZ8F2CpkA)
* [STM32 Embedded Software](https://www.st.com/content/ccc/resource/sales_and_marketing/presentation/product_presentation/37/55/ff/bc/a8/71/4f/c5/stm32_embedded_software_offering.pdf/files/stm32_embedded_software_offering.pdf/jcr:content/translations/en.stm32_embedded_software_offering.pdf)
    ![](https://i.imgur.com/86WxGI6.png)

# Compiler
## Linaro
* [Pre-built GNU cross-toolchain for AArch64 and ARM 32-bit (Windows / Linux / MAC) (Arm Developer website)](https://developer.arm.com/tools-and-software/open-source-software/developer-tools/gnu-toolchain/gnu-rm/downloads)
* [Pre-built LLVM native toolchain for AArch64 and ARM 32-bit (Linux) (LLVM's GitHub)](https://github.com/llvm/llvm-project/releases/)
* [LLVM toolchain for ARM (Windows) (Linaro)](https://github.com/llvm/llvm-project/releases/download/llvmorg-12.0.0/LLVM-12.0.0-woa64.exe)
* [GNU Toolchain Integration Builds](https://snapshots.linaro.org/gnu-toolchain/)


# Debugging Tools
## ST-LINK
* [stlink-org / stlink](https://github.com/stlink-org/stlink)

## SEGGER
### J-Link / J-Trace
* [Ozone — The J-Link Debugger and Performance Analyzer](https://www.segger.com/products/development-tools/ozone-j-link-debugger/)
* [Converting ST-LINK On-Board Into a J-Link](https://www.segger.com/products/debug-probes/j-link/models/other-j-links/st-link-on-board/)
* [J-Link - Models Overview](https://www.segger.com/products/debug-probes/j-link/models/model-overview/)
* [Software and Hardware Features Overview (Version)](https://wiki.segger.com/Software_and_Hardware_Features_Overview)
### Ozone
### SystemView

## Software
### OpenOCD
* [OpenOCD](http://openocd.org/)
* [ 系統架構秘辛：了解RISC-V 架構底層除錯器的秘密！ 系列 ](https://ithelp.ithome.com.tw/users/20107327/ironman/1359?page=1)
* [STM32 GDB/OpenOCD Commands and Initialization for Flash and Ram Debugging](https://stackoverflow.com/questions/5535110/stm32-gdb-openocd-commands-and-initialization-for-flash-and-ram-debugging)
* [How to use the GDB (Gnu Debugger) and OpenOCD for microcontroller debugging - from the terminal?](https://stackoverflow.com/questions/38033130/how-to-use-the-gdb-gnu-debugger-and-openocd-for-microcontroller-debugging-fr)

```
openocd \
-f board/stm32f429discovery.cfg \
-c "init" \
-c "reset init" \
-c "flash probe 0" \
-c "flash info 0" \
-c "flash write_image erase ./build/F429_LED-Blink.bin  0x08000000" \
-c "reset run" \
-c shutdown
```

# IDE
* [Software development toolsSTM32 and STM8 microcontrollers](https://www.st.com/content/ccc/resource/sales_and_marketing/presentation/product_presentation/group0/51/b5/28/37/25/93/48/83/stm32-stm8_software_development_tools.pdf/files/stm32-stm8_software_development_tools.pdf/jcr:content/translations/en.stm32-stm8_software_development_tools.pdf)




