# Getting started on Windows
1. Install ARM GNU for Windows
    * https://developer.arm.com/open-source/gnu-toolchain/gnu-rm/downloads
    * NOT the SHA1 or SHA2 files
2. Install nRF5 SDK for Windows
    * https://www.nordicsemi.com/eng/Products/Bluetooth-low-energy/nRF5-SDK
    * copied and renamed into C:\nRF5
3. Edit `components/toolchain/gcc/Makefile.Windows` to point to GNU
    ```
    GNU_INSTALL_ROOT := C:/Program Files (x86)/GNU Tools ARM Embedded/8 2018-q4-major/bin/
    GNU_VERSION := 8.2.1
    GNU_PREFIX := arm-none-eabi
    ```