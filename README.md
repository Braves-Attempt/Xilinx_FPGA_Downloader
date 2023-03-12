# Xilinx_FPGA_Downloader

# Overview
In this repo you may find the xilinx USB downloader  based on FT232/FT2232/FT4232 three chip design schemes, and firmware programming!

# Include
  - Design Schematic
  - PCB and Gerber files
  - Firmware programming
  
# FT232/FT2232/FT4232 difference
  - FT232  no serial port
  - FT2232 has a serial port
  - FT4232 has three serial ports
  
# Firmware program step
  - Open Xilinx Software Command Line Tool 2022.2
  - Enter the following command(just test)
      FT232:  program_ftdi -write -ftdi FT232H -serial 11053463 -vendor "SZ_TECH" -board "K7_FMC" -desc "XILINX”
      FT2232: program_ftdi -write -ftdi FT2232H -serial 11053463 -vendor "SZ_TECH" -board "K7_FMC" -desc "XILINX”
      FT4232: program_ftdi -write -ftdi FT4232H -serial 11053463 -vendor "SZ_TECH" -board "K7_FMC" -desc "XILINX”
      
# about SCH & PCB
  The design is based on cadence 17.4 version and provides Gerber files
  This hardware design supports FT2232 and FT4232, only one serial port can be used
