# CEITEC-MOTES-public-LV-repo
Public repository for LabVIEW apps developed by CEITEC Magneto-Optical and THz spectroscopy group

## License
GPL v3

## Author
Matúš Šedivý

Copyright (c) Central European Institute of Technology - Brno University of Technology 2022 


## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## 1 Transistor Characteristics
App to sweep gate and drain voltage, and measure drain current (2D data), by two Keithley 2450 SMUs.

### 1.1 Install
- requieres LV driver for Keithley 2450

### 1.2 Usage
Start program, asign Drain and Gate SMU, select measurement parameters, adjust reading delay and active terminals if needed, and click Start measurement.
Measurement will ne done in "chunks" - drain voltage sweep procedure is attomic. If program crashes after first sweep on error related to buffer, try to increase reading delay (bug in a Keithley HW/FW).
