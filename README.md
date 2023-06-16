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
git submodule update --init
```

---
## Configure:
* the deployment.h is a pre-include to all files within the build, edit it to configure build options

---
## Build:
```
make
make program
make debug_openocd
make clean
make scrub
```

---
## Layers:
```
└── ogc_project_nrtps_on_arduino_mega
    ├── README.md
    ├── LICENSE
    ├── Makefile ( control aspecs of the project by using `make` build system )
    ├── deployment.h ( preinclude file that controls several aspects about build )
    ├── software
    │   ├── applications
    │   │   └── ogc_app_demo_blink.git ( application handling a demo blink of an indicator with multi OS support )
    │   └── libraries
    │       ├── ogc_lib_indicator_status_single.git ( library handling binary indicator blink patterns )
    │       └── ogc_lib_os_nrtps.git ( library holding the Non Real-Time Polled Scheduler Operating System )
    ├── firmware
    │   ├── hal
    │   │   └── ogc_hal_arduino_mega_2560_demo.git ( demo abstraction layer linking hardware to software interfaces )
    │   ├── drivers
    │   └── csp
    │       └── csp_atmel_atmega2560.git ( manufacturer csp supporting the Atmel ATMega 2560 )
    └── hardware
        └── ogc_hw_arduino_mega_2560_base_dev.git ( hardware description for Arduino Mega 2560 development base board )
```

