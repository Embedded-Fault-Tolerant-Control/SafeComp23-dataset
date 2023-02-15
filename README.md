# SafeComp23 - Fault Tolerant Control using Dynamic Control Reallocation on a Hexacopter in outdoor test flights
- All motor orders are based on the [DJI conventions](https://forum44.djicdn.com/data/attachment/forum/201711/26/172348bppvtt1ot1nrtp5j.jpg)
  - Referenced from [ArduPilot codebase](https://github.com/ArduPilot/ardupilot/blob/19ff65a4add88e09821a963f41dfe6e6633d0aa8/libraries/SITL/SIM_Frame.cpp#L65)
  - Except for HexaCopter with X frame - which is clockwise and noted as hexa-cwx in the ArduPilot SITL

| Vehicle Type | Frame | Frame Type | Filename
| ----------- | ----------- | ----------- | ----------- |
| Quadcopter | <img src="../../images/quadplus.png" width="200"/> | Plus | M1 [bin](quad-plus/m1.bin) [mat](quad-plus/m1.mat) <br> M2 [bin](quad-plus/m2.bin) [mat](quad-plus/m2.mat)<br> M3 [bin](quad-plus/m3.bin) [mat](quad-plus/m3.mat)<br> M4 [bin](quad-plus/m4.bin) [mat](quad-plus/m4.mat)<br> M1 & M2 [bin](quad-plus/m1m2.bin) [mat](quad-plus/m1m2.mat)<br> M1 & M3 [bin](quad-plus/m1m3.bin) [mat](quad-plus/m1m3.mat)<br> M1 & M4 [bin](quad-plus/m1m4.bin) [mat](quad-plus/m1m4.mat)<br> M2 & M3 [bin](quad-plus/m2m3.bin) [mat](quad-plus/m2m3.mat)<br> M2 & M4 [bin](quad-plus/m2m4.bin) [mat](quad-plus/m2m4.mat)<br> M3 & M4 [bin](quad-plus/m3m4.bin) [mat](quad-plus/m3m4.mat)
| Quadcopter | <img src="../../images/quadx.png" width="200"/> | X | M1 [bin](quad-x/m1.bin) [mat](quad-x/m1.mat) <br> M2 [bin](quad-x/m2.bin) [mat](quad-x/m2.mat)<br> M3 [bin](quad-x/m3.bin) [mat](quad-x/m3.mat)<br> M4 [bin](quad-x/m4.bin) [mat](quad-x/m4.mat)<br> M1 & M2 [bin](quad-x/m1m2.bin) [mat](quad-x/m1m2.mat)<br> M1 & M3 [bin](quad-x/m1m3.bin) [mat](quad-x/m1m3.mat)<br> M1 & M4 [bin](quad-x/m1m4.bin) [mat](quad-x/m1m4.mat)<br> M2 & M3 [bin](quad-x/m2m3.bin) [mat](quad-x/m2m3.mat)<br> M2 & M4 [bin](quad-x/m2m4.bin) [mat](quad-x/m2m4.mat)<br> M3 & M4 [bin](quad-x/m3m4.bin) [mat](quad-x/m3m4.mat)
| Hexacopter | <img src="../../images/hexaplus.png" width="200"/> | Plus | M1 [bin](hexa-plus/m1.bin) [mat](hexa-plus/m1.mat)<br> M2 [bin](hexa-plus/m2.bin) [mat](hexa-plus/m2.mat)<br> M3 [bin](hexa-plus/m3.bin) [mat](hexa-plus/m3.mat)<br> M4 [bin](hexa-plus/m4.bin) [mat](hexa-plus/m4.mat)<br> M5 [bin](hexa-plus/m5.bin) [mat](hexa-plus/m5.mat)<br> M6 [bin](hexa-plus/m6.bin) [mat](hexa-plus/m6.mat)<br> M1 & M2 [bin](hexa-plus/m1m2.bin) [mat](hexa-plus/m1m2.mat)<br> M1 & M3 [bin](hexa-plus/m1m3.bin) [mat](hexa-plus/m1m3.mat)<br> M1 & M4 [bin](hexa-plus/m1m4.bin) [mat](hexa-plus/m1m4.mat)<br> M1 & M5 [bin](hexa-plus/m1m5.bin) [mat](hexa-plus/m1m5.mat)<br> M1 & M6 [bin](hexa-plus/m1m6.bin) [mat](hexa-plus/m1m6.mat)<br> M2 & M3 [bin](hexa-plus/m2m3.bin) [mat](hexa-plus/m2m3.mat)<br> M2 & M4 [bin](hexa-plus/m2m4.bin) [mat](hexa-plus/m2m4.mat)<br> M2 & M5 [bin](hexa-plus/m2m5.bin) [mat](hexa-plus/m2m5.mat)<br> M2 & M6 [bin](hexa-plus/m2m6.bin) [mat](hexa-plus/m2m6.mat)<br> M3 & M4 [bin](hexa-plus/m3m4.bin) [mat](hexa-plus/m3m4.mat)<br> M3 & M5 [bin](hexa-plus/m3m5.bin) [mat](hexa-plus/m3m5.mat)<br> M3 & M6 [bin](hexa-plus/m3m6.bin) [mat](hexa-plus/m3m6.mat)<br> M4 & M5 [bin](hexa-plus/m4m5.bin) [mat](hexa-plus/m4m5.mat)<br> M4 & M6 [bin](hexa-plus/m4m6.bin) [mat](hexa-plus/m4m6.mat)<br> M5 & M6 [bin](hexa-plus/m5m6.bin) [mat](hexa-plus/m5m6.mat)
| Hexacopter | <img src="../../images/hexax.png" width="200"/> | X | M1 [bin](hexa-x/m1.bin) [mat](hexa-x/m1.mat)<br> M2 [bin](hexa-x/m2.bin) [mat](hexa-x/m2.mat)<br> M3 [bin](hexa-x/m3.bin) [mat](hexa-x/m3.mat)<br> M4 [bin](hexa-x/m4.bin) [mat](hexa-x/m4.mat)<br> M5 [bin](hexa-x/m5.bin) [mat](hexa-x/m5.mat)<br> M6 [bin](hexa-x/m6.bin) [mat](hexa-x/m6.mat)<br> M1 & M2 [bin](hexa-x/m1m2.bin) [mat](hexa-x/m1m2.mat)<br> M1 & M3 [bin](hexa-x/m1m3.bin) [mat](hexa-x/m1m3.mat)<br> M1 & M4 [bin](hexa-x/m1m4.bin) [mat](hexa-x/m1m4.mat)<br> M1 & M5 [bin](hexa-x/m1m5.bin) [mat](hexa-x/m1m5.mat)<br> M1 & M6 [bin](hexa-x/m1m6.bin) [mat](hexa-x/m1m6.mat)<br> M2 & M3 [bin](hexa-x/m2m3.bin) [mat](hexa-x/m2m3.mat)<br> M2 & M4 [bin](hexa-x/m2m4.bin) [mat](hexa-x/m2m4.mat)<br> M2 & M5 [bin](hexa-x/m2m5.bin) [mat](hexa-x/m2m5.mat)<br> M2 & M6 [bin](hexa-x/m2m6.bin) [mat](hexa-x/m2m6.mat)<br> M3 & M4 [bin](hexa-x/m3m4.bin) [mat](hexa-x/m3m4.mat)<br> M3 & M5 [bin](hexa-x/m3m5.bin) [mat](hexa-x/m3m5.mat)<br> M3 & M6 [bin](hexa-x/m3m6.bin) [mat](hexa-x/m3m6.mat)<br> M4 & M5 [bin](hexa-x/m4m5.bin) [mat](hexa-x/m4m5.mat)<br> M4 & M6 [bin](hexa-x/m4m6.bin) [mat](hexa-x/m4m6.mat)<br> M5 & M6 [bin](hexa-x/m5m6.bin) [mat](hexa-x/m5m6.mat)



## Sample data

- X-Frame QuadCopter is used
- [15:47:15] Drone starts ascent
- [15:47:55] Goes up to altitude of 100meters
- [15:48:00] Fault introduced in motor 2 (from code)
- Immediately starts descent
- [15:48:15] Crash lands in 15-16 seconds

### Barometer
![](../../images/100m/Barometer.png)

### Gyroscope
![](../../images/100m/Gyro_1.png)

### Roll, Pitch, Yaw
![](../../images/100m/Euler_Roll.png)
![](../../images/100m/Euler_Pitch.png)
![](../../images/100m/Euler_Yaw.png)

### Servo outputs
![](../../images/100m/Servos_1-4.png)