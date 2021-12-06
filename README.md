# Virtex-PCBs

This repository contains the Altium source for Virtex's PCBs and adapter board (34V0-CB-A, 34V0-CB-B, 34V0-CB-C, and 34AB0-CB).

 - Altium Version: 21.8.1


## Board Descriptions

34V0-CB-A "Power Board":
 - USB-C & fixed cable jacks
 - 13.6W LED power supply
 - 3.3V 1.7A for 34V0-CB-B
 - 3.6V image sensor reference voltage (stage 1)

34V0-CB-B:
 - Xilinx Artix-7 FPGA (XC7A35T-1FTG256C)
   - Reads and processes Python 300 LVDS signals into blobs (sent over I2C) and a camera stream (sent over fast serial)
 - Python 300 Infrared-Optimized Image Sensor (NOIP1FN0300A-QDI) 
 - USB 2.0 interface (FT2232HQ)
   -  JTAG on bus A to program the FPGA & flash
   -  Fast Serial on bus B for camera stream

34V0-CB-C "LED Board":
 - 8x 1A 850nm IR LEDs (BWIR-35C2O48)

34AB0-CB "Adapter Board":
- 8:2 Multiplexer (SN74LV4052APWR)
- Weidmuller Omnimate LSF-SMT series connectors

---

If you have any questions feel free to contact us at [info@34engineering.com](mailto:info@34engineering.com)
