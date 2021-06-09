# Configure fuel sensor with GPS device S200/S400

### Step 1: Calibrate the sensor

You can refer to  [here](modules/web-interface/devices/calib-sensor/#calib)

### Step 2: Connect sensor to the GPS tracker
    
<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/faq/wire-2.jpeg)

* RX of Sensor --> TX of S200/S400: Yellow
* TX of Sensor --> RX of S200/S400: Blue

### Step 3: Configure

- Soji sensor sold abroad uses 19200 baudrate

    **Rs232,0,2,19200#**

- Soji sensor sold in Vietnam uses 9600 baudrate

    **Rs232.0,2,9600#**

### Step 4: Save configuration

Send **reset#** command to save and update configuration

### Step 5: Check
    
#### Frequency to read data from sensor, default is 10s
  
  **rs232para,0,10,5#**

#### Check sensor readings

-Wait a few minutes, send command :
 
  **view,comm#**

- After sending the command **view,comm#**, the response content is as shown below:
  - Having index = 0 means that the sensor is connected and readable

  <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/faq/check-connect-sensor-1.jpg)

### Step 6: Configuration on Platform

- First, select the vehicle you want to configure.
  **1.** Click on the <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/file-alt.svg) **Infor** tab of that vehicle. Or click on the icon <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/file-alt.svg)  in the device info box
    
    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/faq/add-sensor-4.jpg)
  
  **2.** Click on <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg)**Add sensor**" tab , the following dialog box will appear:

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-interface/faq/add-sensor-3.jpg)

  **3.** Fill in the information in the dialog box:

  * ***Basic***
    * **Sensor name**: Name your sensor for easy memory and visualization.
    * **Calculation method**: Select 1 of 3 methods: Calibration, Linear, Original.
    * **Input**: Select the corresponding parameter.
    * **Unit**: Select the unit to be measured.
    * **Sensor Type**: Select the sensor type corresponding to the unit of measure.
    - **Calibration** : Enter the correct value as the example (Only appears when the Calibration method is selected)
    **Formula** : Enter the correct value as the example (Only appears when selecting the Linear (linear), Original method)
    - **Min** : Enter the minimum value of the calibration.
    - **Max**: Enter the maximum value of the calibration.
  * ***Advanced*** 
    * **Increase minimum**: Enter sensor value to change when abnormally increase.
    * **Decrease minimum**: Enter sensor value to change when decreasing abnormally.
    * **Offset**: Enter a zero correction value when calculating the ADC to output the correct temperature (sensor type) value.
    * **Round**: Rounds the sensor value by how much after the (,).
    * **Sort**: Sort the change sensor value to any position.
    * **Description**: Can write more information about the sensor, ...
    * **Show map on map**: Turn on / off to show / not show sensor name on the map.

    **4.** Click **Add** to save the sensor.
    
    **5.** Click **Save Changes** to complete the device repair operation.

#### Ask the device to send stat updates to the web

- When the sensor readings have been read on the device, but the value has not been updated on the web, the following command can be used to request the device to send the sensor readings immediately

  **pack,sensor#**