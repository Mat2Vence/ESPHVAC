#ESP HVAC

##Introduction
*This code aims to control a Panassonic HVAC over the internet through WIFI. This project is based on the work I did perform to reverse-engoinner my Mitsubishi HVAC, and which result was intially merged on the Vincent's project (https://github.com/r45635).
*The code is written to work with a nodeMCU plateform (ESP8266 based) for the IoT part. The system is then built in order to work with Domoticz in order to control the HVAC from a global home atuomation system.

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
