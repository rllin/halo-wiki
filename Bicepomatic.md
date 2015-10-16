**Bicepomatic** is an apparatus intended to characterize bicep contraction under dynamic conditions. It is intended for use in MVC-05.

# Safety
### Hard Stop
### Kill Switch

# Muscle Isolation System
### Bench
### Curl Table (Preacher Bench)
### Curl Arm
### Curl Pad

# Drive System
### Driver Motor
* [CPM-MCPV-3441P-RLS](https://www.teknic.com/model-info/CPM-MCPV-3441P-RLS/) - Purchased
 * Depth: 136.5mm
 * Face Dimensions: 86.87mm^2, [[NEMA]] 34
 * Peak torque: 6.51 Nm
 * Peak Speed: 1800 RPM
 * Resolution: 0.45 degrees

### Motor Control
* Computer --> ClearPath-MSP (Program) --> Developer Board (like arduino or MSP) --> I/O 6 Pin Cable --> I/O Input Connector (integrated in controller) --> Controller (integrated in CPM-MCPV Motor)

### Gearing 
Target 10:1, range from 7:1 - 15:1
* Gearbox
 * [Planetary, 5:1, NEMA 34](http://www.automationtechnologiesinc.com/products-page/cnc-gear-box/51-planetary-gearbox-for-automation-systems-4-thousand-rpm)
 * 90 Degree Gearbox would make mounting Motor Easier
* Sprocket Ratio
 * Range from 3.5:1 - 1:3.5 since DriveN Sprocket min teeth ~32, and DriveR Sprocket max ~112

### Belt
* [[HTD]] Belt

### Sprocket
* DriveR
 * P32-5MGT-25-MPB (PN: 7709-2112 ) PowerGrip GT2, 5mm pitch, 25mm wide, Bore 1/2" - 15/16",Steel
* DriveN
 * P112-5MGT-25 (PN: 7709-2112 ) PowerGrip GT2, 112 teeth, 5mm pitch, 25mm wide, Bore 1/2 - 2 1/8", Ductile Iron
 * Coupling - Use Clamping Style Coupling, according to [Teknic ClearPath User Manual](https://www.teknic.com/files/downloads/clearpath_user_manual.pdf)

# Data Collection System
### Velocity/Position Gauge
* Encoder, Integrated in Driver Motor [CPM-MCPV-3441P-RLS](https://www.teknic.com/model-info/CPM-MCPV-3441P-RLS/)

### Force/Torque Gauge
* Integrated in Driver Motor [CPM-MCPV-3441P-RLS](https://www.teknic.com/model-info/CPM-MCPV-3441P-RLS/)
* Dynamometer affixed to Curl Pad

## COST
* Purchased
 * Bicep Curl Bench - $375
 * Driver Motor (Servo) - $500
 * Power Supply - $199
 * Motor Accessory Cables (3) - $56
* Projected
 * Driver Sprocket - $50
 * Driven Sprocket - $50
 * Synchronous Belt - $90
 * Gearbox - $480