# OGC.Engineering
## ogc_project_thermal_inspection_tool
Developer contact - dustin < at > ogc.engineering

---
Location:

- Project Documentation:
    - location: projects/ogc_project_thermal_inspection_tool/
    - repo: https://github.com/OGC-dustin/ogc_project_thermal_inspection_tool
- Deployment:
    - location: project using nrtps and basic application
    - repo: 
- Application
    - location: [ basic application operation modes ]
    - repo(s): 
- Libraries
    - location: [ nrtps os, graphical management,  ]
    - repo(s): 
- Firmware Drivers ( Provides hardware specific support in terms of interfacing, sequences, protocols, preprocessing, etc. ):
    - location: [ oled, encoder, color camera, ir camera, lidar, neopixel ]
    - repo(s): 
- Firmware CSP ( Chip Support Package - provides hardware specific manufacturer support for family of controllers ):
    - location: 
    - repo: 
- Firmware HAL ( Hardware Abstraction Layer - Collects all things hardware and interfaces them to software... ):
    - location: 
    - repo: 
- Hardware Definition ( Describes the physical hardware and needed resources ):
    - location: hardware/ogc_hw_thermal_inspection_tool/
    - repo: https://github.com/OGC-dustin/ogc_hw_thermal_inspection_tool

Purpose:
- Development platform for image capture ( RGB and Thermal ) use in various inspection tasks

Use cases:
- Identification of thermal hot spots
- Aggregate distance measurement to landmark
- Color reflection analysis ( including IR light source )

This project is also acting as a demonstration project illustrating layered development for speed and maintainability.

---
Milestones:
- ( COMPLETE 20230330 ) Blink LED - Prove you have control over GPIO and code is running
- UI Board - OLED, SDCard, Encoder, RGB LED
    - build UI board
    - set up encoder interrupts, driver ( track position, direction, etc. )
    - set up rgb led status indicator ( gpio versus pwm control and driver for color mixing, library to drive patterns, color fades, etc. )
    - set up oled driver ( init, reset, draw primitives, etc. )
    - set up sd card driver ( file format?? )
- Sensor Board - RGB Camera, IR Camera, LIDAR, NEOPixel Ring
    - build sensor board ( will need external power for certain items )
    - set up RGB camera
    - set up IR camera
    - set up lidar
    - set up NEOPixel
- Application...  define how the device should act and the different modes of operation