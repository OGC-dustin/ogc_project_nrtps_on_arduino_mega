# OGC.Engineering
## ogc_project_nrtps_on_arduino_mega
Developer contact - dustin ( at ) ogc.engineering

---
## Description:
* Demonstration project for using the NRTPS OS on an Arduinio Mega 2560 development platform

---
## Cloning the repository:
```
git clone https://github.com/OGC-dustin/ogc_project_nrtps_on_arduino_mega.git
cd ogc_project_nrtps_on_arduino_mega
git submodule init --update
```

---
## Build the project:
```
make
```

---
## Program the device:
```
make program
```

---
## Debug the device:
```
make debug
```

---
## Layers:
```
└── ogc_project_nrtps_on_arduino_mega
    ├── README.md
    ├── LICENSE
    ├── software
    │   ├── applications
    │   └── libraries
    │       └── ogc_lib_os_nrtps.git
    ├── firmware
    │   ├── drivers
    │   ├── hal
    │   └── csp
    └── hardware
        ├── ogc_hw_arduino_mega_daughter_dev.git
        └── ogc_hw_arduino_mega_2560_dev_base.git
```

