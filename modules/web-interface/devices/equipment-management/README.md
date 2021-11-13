# Other functions

### 1. Move/Sell device

To start performing the **Search** function, users go to **Manage > Devices**

<span class="icon-left4">![active device ](/docs/assets/images/web-english/device/manage-device.png)

To move/sell a device to another account, there are 2 options :

* **Option 1** :

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/move-device-1.png)

    - Step 1: Tick the device to move/sell.
    - Step 2: Choose **Move/Sell.**
    - Step 3: A dialog box appears. Select the **account** to move/sell the device to. The **IMEI** is the number of that device.
    Click **Submit** to move/sell the device.
 
* **Option 2** :

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/move-device-2.png)

    - Step 1: Click More

    - Step 2: Select **Sell device & Create user**.

    - Step 3: Enter the information in the dialog box

        - **Account**: Select an account to sell the device for.
        - **Account prefix**: Corresponding to the selected account.
        - **Role**: Select the role of the account.
        - **IMEI**: Number of that device.

    - Step 4 : Click **Submit** to sell the device.

### 2. Active/Disable device

* Automatic activation: The device is automatically activated after 8 hours after its creation and installation.
* Manual activation:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/active-device.png)

    - Step 1: Select the device you want to active/disable.

    - Step 2. Select :point_right:  active/disable. The IMEI is the number of that device.

    - Step 3: A dialog box appears. The status setting is active/disable. The IMEI is the number of that device.

    - Step 4 : Click **Submit** to active/disable device.

### 3. Set device status

- To install the status for device, performance the following step:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/status-device.png)


  - Step 1: Tick the device that needs a status setting.
  - Step 2: Select **Status**.
  - Step 3: A dialog box appears. Select **the correct current status** of the device. The **IMEI** is the number of that device.
  - Step 4 : Click **Submit** to set the status of the device.

### 4. Send command

- To send device command, do the following:

    <span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/device/send-command.png)

  - Step 1: Tick the device to send the order.
  - Step 2: Select **Send command**.
  - Step 3: A dialog box appears. Device name, Device type created. Select **command type** of order to be executed.

  - Step 4 : Click **Submit** to send the device command.


    For more details, please refer [here](modules/web-english/devices/send-the-device-command/#command)  <div id="command"> 

### 5. CCID
- Check if the SIM installed on the device is a valid SIM or not.
- CCID Origin is the SIM attached when exporting and can be updated when there is a change request.
- CCID is the current SIM attached to the device.
- A valid SIM is a SIM with CCID equal to CCID Origin.
- Invalid SIM is a field whose CCID is not equal to CCID Origin + CCID check must be enabled + CCID must be provided by GoTrack and exist in the SIM management system.

#### 5.1. Sync CCID
- **Option 1**
  - Is **updating CCID Origin = CCID**

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/ccid-sync.png)

  - Step 1: Tick select **IMEI** to sync CCID.
  - Step 2: Click **CCID > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Sync CCID**.
  - Step 3: **Check IMEI**.
  - Step 4: Click **Send** to sync CCID.
- **Option 2**

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/ccid-sync-2.png)
  
  - Click icon **<span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Sync CCID** of that device.

#### 5.2. Update check CCID
- Is **allow to enable/disable SIM check**

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/update-ccid-check.png)
  - Step 1: Tick select **IMEI** to update check CCID.
  - Step 2: Click **CCID > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Update check CCID**.
  - Step 3 :
    - **Status** : Activate/Deactivate to enable/disable SIM.
    - **IMEI** Device to be tested.
  - Step 4: Click **Send** to update CCID check.


#### 5.3. Update CCID:
- Allow manual CCID update.

    <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/update-ccid.png)
  - Step 1: Tick select **IMEI** to update CCID.
  - Step 2: Click **CCID > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Update CCID**.
  - Step 3 :
    - **IMEI** Device to be tested.
    - **CCID** is the code printed on the SIM card. The current SIM is attached to the device

  - Step 4: Click **Send** to update CCID.

### 6. More
#### 6.1. Reset location
- If the location of the device is not available, you can quickly configure it here.
  <span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/reset-location.png)

  - Step 1: **Select the device** to set the location
  - Step 2: Go to **Add > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg) > Reset location**.
  - Step 3: Dialog box opens. Enter information in the form:
    - **Latitude** is the value that determines the position of a certain point on the surface of the Earth and including other planets, north or south of the equator.
    - **Longitude** is the geographical coordinate value in the east to west direction.
    - You can go to Google Maps to get exact coordinates.
  > Note : Only integer coordinates can be entered.
  - Step 4: Press **Send** to reset the position.

#### 6.2. Swap IMEI
- When the customer's car is changed to a new device, if you want to change the IMEI on the system to display the data according to the new IMEI, do the following:
<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/change-imei.png)
  - Step 1: **Select device** need to change IMEI.
  - Step 2: Click **Add > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg ) > Swap IMEI**.
  Step 3: A dialog box will appear. Fill in the information in the form.
    - **New IMEI** : Enter the new IMEI that is already in stock.
  - Step 3: Click **Save Changes** to change IMEI.

#### 6.3. Reset factory
- When you want to save new data from the beginning / have a problem that needs to be reset to default, do the following:
<span style="display:block;text-align:left">![Manage device ](/docs/assets/images/web-english/device/reset-to-defaults.png)
  
  - Step 1: **Select the device** to be Reset factory
  - Step 2: Click **Add > <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/ellipsis-h.svg ) > Reset factory**.
  Step 3: A dialog box will appear. Fill in the information in the form.
    - **IMEI** : Enter IMEI that is already available in stock / add IMEI to reset to default and check that IMEI again.
  - Step 3: Click **Send** to change IMEI.

