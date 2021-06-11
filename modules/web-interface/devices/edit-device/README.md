# Edit decvice 

<div id="suathietbi">
</div>

To start performing the **Edit** function, users go to **Manage > Devices**

<span class="icon-left4">![active device ](/docs/assets/images/web-english/device/manage-device.png)

When you click on <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-edit.svg) **Edit**  of that device, a dialog box will appear as follows:

<span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/basic-edit.png)

### Basic
* ***Device Information*** 

    * **IMEI**: Identification number of the device. (Editing is not allowed).

    * **Account**: Your account name/username. (Editing is not allowed).

    * **Icon**: Click on the box below to select the icon of the vehicle/vehicle where you are installing the device.

    * **SIM number**: Enter the phone number you are using.

    * **Device Name**: The device name can be changed to make it easy to remember and see.

    * **Device type**: Select the device type name corresponding to the device you are using.

    * **Device group**: A group of devices that share something in one account.

        <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-device-group.png)

        * Step 1: Click <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) to add the device group.

        * Step 2: Select the account you want to add the device group too. Enter the device group name.

        * Step 3: Click **Add** to complete the operation.

        Besides, you can create more device groups by doing the following:

        <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-device-group-2.png)

        See more details about the **Device Group** [here](modules/web-interface/configuration/device-group/#device-group) <div id="device-group" >

    * **SIM type**: Select a SIM type corresponding to the carrier of the phone number.
* ***Services*** 
    * **Service term**: Term of service.
    * **Activate**: Can turn on / off when you want/don't want to use the service.

* ***Warranty*** 

    * Activate warranty: Can be on / off.
    * Warranty activation date: Activation date of device warranty.
    * Warranty period: The equipment warranty expiration date according to the warranty package of that service.
    * Notes: Type a note if you want to annotate something.

* ***Sell info*** 

    * **Sold**: When the device has been sold to the account, it will turn on automatically. If not, it will be turned off.
    * **Sell date**: Set the date to sell the device to another account (if applicable).
    * **Updated time**: The system automatically updates the date of selling the device when there is a change. 


### Advanced



<span class="icon-left4">![active device ](/docs/assets/images/web-english/device/advanced-edit-device.png)

* ***Vehicle information***

    * **License plate**: Variable vehicle for which the navigation device is installed.

    * **VIN number**: The chassis number consists of 17 characters. (For cars).

    * **Distance factor**: Distance in km in 1 vector unit By default, the distance factor is 1.0.

    * **Frame number**: Vehicle identification number. A series of sequences and characters were chiseled on the chassis.

    * **Engine number**: The engine number of your vehicle.

    * **Driver**: The name of the driver of the vehicle/vehicle with the positioning device installed. If not, click on <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg)

        <span class="icon-left4">![active device ](/docs/assets/images/web-english/device/add-driver.png)

        * **Account** : The name of the account you want to add the driver to.

        * **Name** : Name of the driver who installed the device.

        * **Phone number** : The driver's phone number.

        * **License number** : Class of driver's license.

        * **Issued date** : Date of issuance of the driver's license.

        * **Expired date** : The expiration date of driver's license.

        * **Code** : Driver's license code.

        * **Email** : Driver's email.

        * **Address** : Driver's address.

        * **Description** : Describe more necessary information, ...

        Click **Add** to save the driver.

        Alternatively, you can add drivers by doing the following:

        <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-driver-2.png)

        See more details about the **Driver** [here](modules/web-interface/configuration/driver/#driver) 
  
* ***Fuel***

    * Consumption norm (liter / 100km): Set a vehicle fuel consumption limit for how many liters / 100km.

* ***Advanced features***

    * **Toll station**: Can be switched on / off. When turning on when the vehicle passes through toll booths, a warning will be made and how much will it cost the vehicle to pass through, corresponding to the type of transport.
    * **Type of transport**: Choose 1 out of 5 types of transport. (Only applicable in Vietnam)

* ***Ministry of Transportation***

    * **Send data**: Can be enabled/disabled.
    * **Province**: Select a province to send data. (Selected only when sending mode is enabled).
    * **Transport type QCVN**: Choose one of the types of transport that is correct for the vehicle/vehicle in which you install the equipment. (Selectable only when sending mode is enabled).


<div id="sensor">
</div>

### Sensor

* Before adding new sensors, see the diagram below, how parameters are sent from the gps device and how they need to be paired with the sensors.

    <span class="icon-left6">![active device ](/docs/assets/images/web-english/device/sensor-device-2.png)

* Choose "<span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) **Add sensor**" tab , the screen will display as follows:
 
    <span class="icon-left6">![active device ](/docs/assets/images/web-english/device/sensor.png)

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-sensor.png)

#### Basic
    
* **Sensor name**: Name your sensor for easy memory and visualization.
* **Calculation method**: Select 1 of 3 methods: Calibration, Linear, Original.
* **Input**: Select the corresponding parameter.
* **Unit**: Select the unit to be measured.
* **Sensor Type**: Select the sensor type corresponding to the unit of measure.
- **Formula** : Enter the correct value as the example (Only appears when selecting the Linear (linear), Original method)
- **Minimum** : Enter the minimum value of the calibration.
- **Maximum**: Enter the maximum value of the calibration.

#### Advanced 

* **Increase minimum**: Enter sensor value to change when abnormally increase.
* **Decrease minimum**: Enter sensor value to change when decreasing abnormally.
* **Offset**: Enter a zero correction value when calculating the ADC to output the correct temperature (sensor type) value.
* **Round**: Rounds the sensor value by how much after the (,).
* **Sort**: Sort the change sensor value to any position.
* **Description**: Can write more information about the sensor, ...
* **Show map on map**: Turn on / off to show / not show sensor name on the map.

    Click **Add** to save the sensor.

### Camera 

#### For camera type: Basic

* Choose "<span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) **Add camera**" tab , the screen will display as follows:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-camera-2.png)

  * **Name**: Enter the name of the camera you want to install.
  * **Camera type**: Select Basic  only captures pictures.
  * **Camera Id**: Enter the code of the camera.
  * **Description**: Can enter more information about the camera, ...

<div id="cameraplay">
</div>

#### For camera type: MDVR

* Choose "<span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) **Add camera**" tab , the screen will display as follows:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-camera-6.png)

  * **Name**: Enter the name of the camera you want to install.
  * **Camera type**: **MDVR** in addition to taking pictures also has a video recording feature.
  * **MDVR Id**: ID printed on SM400 device.
  * **Host**: IP address or camera server access domain name.
  * **Port**: Connection port to the camera recorder. Default is 6605.
  * **Channel** : The camera cable plugs into the port of any channel, then select that channel.

    - Mounting channel position at the recorder, **AV1  <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg)  AV4**. (For 8-channel recorders, **AV8** ).
    - Corresponding from **CH1 <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) CH8**
    - Only 1 channel can be created.

  * **Position**: For vehicles that transmit data to the Ministry of Transport, it is mandatory to install cameras at the following 3 locations:

    - **Driver** : The location where the driver or driver is seen.
    - **Door**: Position of passengers getting on and off the vehicle.
    - **Passenger**: The position covers all passengers on the vehicle.
  * **Description**: Can enter more information about the camera, ...
  * **Replication**: If you want to create multiple channels at the same time, choose to clone, copy that channel. To save time and create channels faster. When cloning is successful, just select the channel number again

    Click **Add** to save the camera.


### Extension
<span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/extension-device.png)

* **Confi**

    * **Timeout GPRS (minute)**: Configure the time to not use the device less than the number that the device is still active.

    * **Stop duration (second)**: Configure the minimum stopping time. If during that period it will not be counted as a stopped vehicle.

    *  **Min speed filter(km/h)**: Filtering the most accurate noise. To determine whether the vehicle is stopping/going.
       *  If the vehicle has a speed < Min speed filter (km/h), it will be counted as a stopped vehicle.

    * **Time zone**: Select the local time zone.

    Besides, the device can be configured by the following figure:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/extension-device-2.png)

### Alert

<span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/alert.png)

* Tick  <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square1.svg) to enable/disable device alerts that you want to send alerts on. 

* Besides, the device can be configured by the following figure:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/alert-device-2.png)