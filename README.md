#ESP HVAC

##Introduction
*This code aims to control a Panassonic HVAC over the internet. This project has been achieved with the help of Vincent Cruvellier (https://github.com/r45635) and this code is based on the version he built for his Mitsubishi HVAC.
*This code was initially developed to work with classical Arduino board and has been then ported to an ESP based board.
*Note the the reverse engineering of the HVAC protocol has been managed using AnalySIR software.

*This code is code is published under Creative Commons license : CC-BY-NC-SA


#Overview of Protocol and features managed
## Panasonic HVAC

the function to send configuration is
```
void sendHvacPanasonic(
 HvacMode                  HVAC_Mode,           // Example HVAC_HOT  HvacPanasonicMode
 int                       HVAC_Temp,           // Example 21  (°c)
 HvacFanMode               HVAC_FanMode,        // Example FAN_SPEED_AUTO  HvacPanasonicFanMode
 HvacVanneMode             HVAC_VanneMode,      // Example VANNE_AUTO_MOVE  HvacPanasonicVanneMode
 HvacProfileMode           HVAC_ProfileMode,    // Example QUIET HvacProfileMode
 int                       HVAC_SWITCH          // Example false
);
```
