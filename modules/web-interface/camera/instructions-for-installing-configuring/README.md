# Instructions for installing and using MDVR (SM400)

### Step 1: Prepare the hardware
- Recorder device SM400 Basic or Livestream.
- Equipment conforms to QCVN31 S200 or S400 standards.
- Camera.
- 4G sim for SM400 livestream recorder (if any).
(SM400 base recorder is not required).
- 4G sim for QCVN31 standard equipment.
- Power cord to connect standard equipment and recorder.
- And other accessories included: RFID card, SD card, GPS antenna, GSM (if any).
- Prepare tools:
  - TFT LCD HD Screen Integrated Car CCTV (7inch): For convenience when updating firmware/configuration or when handling errors.
  - USB at least 1G : Save firmware and configuration files.
    
    <span class="icon-left6">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/lcd-hd.jpg)
  
  <span class="icon-left6">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/usb.jpg)

* **Devices to install SM400 Basic as shown below:**

    <span class="icon-left6">![Manage device ](/docs/assets/images/web-interface/livestream/mdvr-photo.jpg)

* **Devices to install SM400 Livestream as shown below:**

  <span class="icon-left6">![Manage device ](/docs/assets/images/web-interface/livestream/mdvr-live.jpg)

### Step 2: Connect the wires

- Applicable to both SM400 Basic and Livestream recorders
     - Plug in a cable with a QCVN-compliant device connector to the SM400 recorder.

    <span class="icon-left16">![Manage device ](/docs/assets/images/web-interface/livestream/connect-sm400-s200.jpg)

     - Plug the camera into the recorder in order from AV1 <span class="icon-left svg-filter-serch">![Ok](/docs/assets/images/web-interface/icon/SVG/arrow-right.svg) AV4
     - Insert the SD memory card into the SM400 recorder.
     - Insert 4G sim (only for SM400 livestream) into the SM400 recorder.
     - Connect the SM400 recorder to the monitor for configuration.
     - Power on the SM400 recorder.

### Step 3: Configure the recorder

**(Only for SM400 Livestream)**

* **Camera Server IP Settings**

    <span class="icon-left12">![Manage device ](/docs/assets/images/web-interface/livestream/ip-camera-1.jpg)

* **Video save mode setting**
  
* **Video settings: basic settings, main stream settings, sub stream settings, timing settings, storage management, OSD settings**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/record.png)

    * **Basic setting: basic recording parameter setting**

        <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/general.png)

        *	Video format: PAL, NTSC, press【OK】key to select from the drop-down menu.
        *	Video mode: boot video, timed video, alarm video, Start-up recording: start recording automatically when the device is turned on.Timing recording: start recording during the set timing recording time period, and not recording at other times. Alarm recording: the device starts recording when an alarm is generated.
        *	Audio format:  G726-M40K/G726-M32K/G726M40K/G726M32K/G711A.
        *	Audio gain: 0-14 levels optional, adjust the volume.
        *	Alarm pre-recording: record a period of time before the alarm.
        *	Alarm delay: the recording will continue after the alarm is removed, and the recording time is the set time.
        *	Alarm protection: In the video file list interface, select the video file to lock, it will not be automatically overwritten during the alarm protection.
        *	Camera type: Choose according to the camera resolution.

    * **Main stream setting: setting of recording parameters for each channel**

        <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/main-rec.png)

        *	Channel name: preview and playback screen will be displayed.
        *	Main recording: On: means the channel has the recording function on.

        ```
             Off: means that the channel does not record.
        ```

        *	Resolution: 720P, D1, HD1, and CIF can be selected. For example, under PAL system: 720P resolution is 1280 * 720 , D1 resolution is 704 * 576 , HD1 resolution is 704 * 288, CIF resolution is 352 * 288 .
        *	Frame rate: indicates the number of video frames per second, PAL system is 1 ~ 25 frames/sec, NTSC system is 1 ~ 30 frames/sec```.
        *	Picture quality, picture clarity, 1~8 levels, level 1 picture quality is the highest.
        *	Recording: Turn on/off,indicating whether to record audio while recording video.

    * **Sub-stream settings: set the parameters of the 4G network transmission video stream**

        <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/sub-rec.png)

        *	Sub video: turn on/off, whether to turn on the sub stream video function。
        *	Resolution: CIF/HD1/D1 optional
        *	Frame rate/picture quality/recording: same as the main stream setting interface parameters.

    * **Timing setting: set the timing recording time period**

        <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/time-rec.png)

        *	You can set up to 4 recording time periods per day
        *	Date: The set time period is valid for 7 days from Monday to Sunday
        *	Time zone: the start time of the time zone cannot be greater than the end time.

  * **Storage management：**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/disk-manage.png)

    * Purpose: Optional main video/sub video, select video stream.
    * Priority: high/medium/low;

  * **OSD setting: superimposed information and display position of video recording**

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/osd-set.png)

    *	Superimposed items: time/license plate/phone number/channel number/GPS information.
    *	Enable: open/close.
    *	X/Y coordinate: the position where the superimposed information is displayed on the screen.

### Step 4: Configure the camera on the platform

#### 4.1. Recorder SM400 Basic

* You go to https://gps.gotrack.vn to log in.
  
  **1.** Click on the <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/file-alt.svg) **Infor** tab of that vehicle. Or click on the icon <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/file-alt.svg)  in the device info box
  
  **2.**  Click **Camera > <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) Add camera**, the following dialog box will appear:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-camera-device-5.png)

    * **Name**: Enter the name of the camera you want to install.
    * **Camera type**: Select Basic  only captures pictures.
    * **Camera Id**: Enter the code of the camera.
    * **Description**: Can enter more information about the camera, ...
    
  **3.** Click **Add** to save the camera.
   
  **4.** After configuring the information, click **Save Changes** to complete the operation.

#### 4.2. Recorder SM400  Livestream

* You go to https://gps.gotrack.vn to log in.
  
  **1.** Click on the <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/file-alt.svg) **Infor** tab of that vehicle. Or click on the icon <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/file-alt.svg)  in the device info box

  **2.** Click **Camera > <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/plus.svg) Add camera**, the following dialog box will appear:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/add-camera-4.png)

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

  **3.** Click **Add** to save the camera.

  **4.** After configuring the information, click **Save Changes** to complete the operation.

### Step 5: Configure QCVN

#### 5.1. Configuration of receiving images

**Configure to receive images according to SMS commands sent from the S200/S400 device**

- RS232 port
  
   **rs232,0,9,115200 #**

- Shooting frequency: 300 seconds

    **rs232para,0.300.0 #**

- Server and image upload path:

  * server,file,__ photos.gotrack365.com,80__# or * server,file,__125,212.235.150,9191 __#

  * server,path,__/api/receive-photos__ #

  * __reset #__


#### 5.2. Server settings
* Install connection hub **server**

    <span class="icon-left12">![Manage device ](/docs/assets/images/web-interface/livestream/ip-camera-1.jpg)

    <span class="icon-left12">![Interface Web](/docs/assets/images/integrated-devices/smc/sm400/bb-sv.png)

    *	Monitoring server settings: report the IP address of the video server (main IP connected to the monitoring center).
    *	Ministry standard server setting: Ministry standard protocol platform parameter setting, divided into main server and backup server, and other slaves, expansion server.

### Step 6: Check photos and videos

#### 6.1. Check photo

* Go to Photo Report to see photos
  You go to **Camera > Photo History**.
  The screen displays as shown below:

  <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/livestream/history-image-1.png)

  See details [here](modules/web-interface/camera/history-image/)

#### 6.2. Check out the video

After configuration is complete:
* Step 1: Go to **Camera > Live stream** to view the video camera.
* Step 2: Select a vehicle with camera configuration. Click on **a certain channel > Play all**.

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/livestream/livestream-1.png)

    See details [here](modules/web-interface/camera/livestream/)

* To view the camera video again, go to **Camera > Playback**.
    
    The screen displays as shown below:

     <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/livestream/play-back-1.jpg)
    
    See details [here](modules/web-interface/camera/playback/)
