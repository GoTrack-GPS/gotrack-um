
#  Wiring diagram

### 1. Wiring diagram of SD video recorder

&emsp;<span class="icon-left6">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/diagram-sd.png)

### 2.	Wiring diagram of HDD video recorder

&emsp;<span class="icon-left6">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/diagram-hdd.png)

### 3. Quick setting

#### 3.1. Wiring test and boot

* The power supply of the host has three wires, red, black and yellow. The red and black wires are directly connected to the car battery, the red wire is connected to the positive electrode, the black wire is connected to the negative electrode, and the yellow wire is connected to the ignition wire (ACC). If you test indoors, the red and yellow wires can be connected together. Positive pole, then directly use DC12V power supply.
  
  **1.** Check that the power cord is connected normally, and confirm that the key block is turned on to the LOCK file after the line is connected, then it will start normally, and the power light will be blue after the normal start.

  **2.** Connect the output line AV-OUT to the display screen and connect the corresponding equipment to the terminal. Confirm whether the connection is correct. The following figure shows the actual installation power supply wiring:

&emsp;<span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/power-cable.png)

&emsp;<span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/car-battery.png)

#### 3.2. Vehicles quickly report to the server

> Note: For hosts without WIFI and 3G module functions, the following descriptions are  invalid and do not need to be reported to the platform. 
* Step 1: Install the SIM card, select the SIM card according to the corresponding module.
* Step 2: Boot into the system menu, first modify the mobile phone number in the terminal settings (that is the unique ID of the reporting server) and then modify the corresponding license plate number.
* Step 3: Enter the important network settings, modify the corresponding IP and port number according to the different server deployment IP of each customer, and select the platform of the standard protocol, select the main GPS server on the next page to modify the IP and port number .

&emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/terminal-sv-.png)

#### 3.3. IO serial port use 

* The device has 4 alarm inputs and 2 alarm output interfaces. The alarm input detection is all level detection, which can be connected to various vehicle driving states, such as brake, steering, vehicle switch, and alarm button, as shown in Figure 4-2. 

    &emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/+12V.png)

* When the brake plate is stepped on, MDVR can detect the high level, otherwise the low level, the alarm output is all level output, and the drive capacity is 200mA. If you connect a larger power device, you must connect a relay. As shown in Figure 4-3:
  
    &emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/24V.png)

#### 3.4.  PTZ connection and settings

* Setting steps:
  
  * **First** ：choose the PTZ protocol: PELCO-D and PELCO-P respectively.
  * **Second**：set the baud rate and select it on the terminal according to the corresponding baud rate of the PTZ.
  * **Third**：set the address code: directly enter the address code corresponding to the PTZ address value.
  * **Fourth** wiring: the 485 control line on the PTZ is connected to RS485-A positive, the other one Connect to RS458-B negative.

&emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/method1.png)

&emsp;<span class="icon-left09">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/method2.png)
