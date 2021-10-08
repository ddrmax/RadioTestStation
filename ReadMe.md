# WORK IN PROGRESS


## Non Commercial Hardware and Software to make a Communication System Analyzer Service Monitor under the 1000$ Pricetag for Radio Amateurs to calibrate and test their Radios



### Brains of the machine:
CPU: Raspberry-PI 4 4GB (at least / 8GB recommended)
OS Storage: 64GB SDCard for OS
Media Storage aka "Inernal Storage" 8+GB USBDisk for internal Storage

### External Parts: 
  - Case (Metal / 3D printed / ABS / Wood / Any other sturdy material)
  - Generic Laptop PSU (mini 19V 65W) with corresponding receiving PLUG
  - 10 inch Raspberry Pi TouchScreen
  - Handle
  - Poutch
  - DB9 or DB15 for Radio accessory interface
  - USB extension for faceplate mounting
  - N RF Extension Cable for faceplate mounting x3
  - BNC RF Extension Cable for faceplate mounting x3
  - RJ 45 Extension cable for faceplate mounting x2 (One For LAN / Other One For MIC)
  - Motorola Compatible Handheld Microphone (With RJ45 plug, either Standard or with Keypad)

### Other Misc Internal Parts:
  - USB Hub (number of ports and external powering still needs to be determined)
  - speaker or amplified speaker
  - latest version of the MMDVM board supporting analog FM ( with STM 32 4xx MCU)
  - the small PCB or the big PCB (the big PCB integrates all the MMDVM hardware)



### Other Optional Parts: (not included in the 1000$ price limit)
- Laptop Battery or custom made 3S lithium battery (or a 7Ah AGM if you want it Heavy and Bulky)
- SDR key or HackRF One to use add the spectrum analyser capabilities

### Circuitry breakdown 

External Sound Genreator: STM32" Blue Pill" with addon PCB using Analog Devices IC as parametric sound generator / capture device for Radios accesory ports
RF Capture / Decoder / Generator for Analog and Digital Signals: Original MMDVM Board with STM32 4XX microprocessor or nucleo Board (to support analog as the STM32 1XX doesn't support that feature)

RF mesure and generation provided by Analog Devices and Phillips power ICs
Low power RF circuitry inspired by the MMDVM Hotspot and High power RF circuitry inspired by wavetek and motorola schematics and newer RF ICs schematics in their datasheets



### What are the expected capabilities:
  - Generate and mux analog audio with RF wave
  - Receive and demux analog audio with RF wave
  - Generate Radio frequencies from 0dBm down to -130 dBm
  - Receive Radio frequencies up to 30W
  - show input and output levels of tested devices in real time
  - Generate 1Khz signal with adjustable distortion
  - Generate CTCSS (PL) / DTCSS (DPL) / Selcall (ZVEI / CCIR / EEA )

### What are the optional capabilities that could put the price over the budget
  - Digital support (As to be legal, voice encoding and decoding in most digital modes need a DVSI AMBE USB Stick)
  - Spectrum analyser: SDR key or more capable device that can go over budget
  - VNA 
  - 












Link references:

https://www.qsl.net/va3iul/Homebrew_RF_Circuit_Design_Ideas/Homebrew_RF_Circuit_Design_Ideas.htm

[No Link] Wavetek / Stabilock 4015 and 4031 Schematics from Service Manual (For circuit design considerations, since 3/4 of the parts are not produced anymore

https://blog.qscope.org/2014/02/19/un-wattmetre-rosmetre-open-source-par-tf3lj-ve2ljx/

[No Link] Motorola R2600 User interface (As a UI Base)

