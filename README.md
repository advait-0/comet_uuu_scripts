# UUU Scripts

This repository contains scripts designed to work with **[UUU (Universal Update Utility)](https://github.com/nxp-imx/mfgtools)** to flash various components of the Comet, including **[U-Boot](https://u-boot.org/)** bootloader, and system firmware.

---

## Prerequisites

Before using these scripts, ensure the following:

- UUU (Universal Update Utility) installed on your host machine.  
  You can download it from the [NXP UUU GitHub repository](https://github.com/NXP/uuu).
- USB connection between your host machine and the Comet board.
- All required firmware, bootloader, and image files available on your host.
- Proper serial terminal setup (for debugging or monitoring, e.g., `minicom` or `screen`) with the correct baud rate (usually `115200`).

---

## Usage

1. Connect the Comet board to your host via USB.
2. Open a terminal and navigate to this repository.
3. Run the appropriate script with UUU. For example, to flash the U-Boot image:

```bash
uuu -b -v flash_bootloader.lst
```