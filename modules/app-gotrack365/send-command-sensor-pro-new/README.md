# Send command check sensor connection on app GoTrack365

This sending feature is only for :
- Distributor type account.
- Device S400.

To send the command, perform the following steps:

<span class="icon-left5">![Interface Web](/docs/assets/images/web-english/gotrack365-el/send-command-sms/commands-1.jpg)

- Step 1 :
    - Log in to your Distributor account.
    - Search for the device you want to send commands.
    - Then select the device you want to send the command to on the **Vehicles** screen.

- Step 2: Slide the horizontal menu to select **Send command**.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-english/gotrack365-el/send-command-sms/commands-2.jpg)

- Step 3: Configure baudrate
    - Click on <span style="color:orange"> @</span> on the screen.
    - Select sample command: **Set baud rate**. The command name will automatically appear on the screen.

    > **< RS232 > : is the RS232 port location, 0 is RS232_0 in port A, 1 is RS232_1 in port B <br>
    < SENSOR > : is the sensor type, where 2 is SOJI**
    
    Replace the values ​​according to the formula displayed on the screen.
    - Soji sensor sold abroad uses 19200  baudrate

        **Rs232,0,2,19200#**

    - Soji sensor sold in Vietnam uses 9600  baudrate

        **Rs232.0,2,9600#**
    - Press <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) to Send command.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-english/gotrack365-el/send-command-sms/commands-3.jpg)

- Step 4: Check the frequency of reading data
    
    - Click on <span style="color:orange"> @</span> on the screen.
    - Select sample command: **Set sensor update interval**. The command name will automatically appear on the screen.
        
        Replace the values ​​according to the formula displayed on the screen.

    - Frequency of reading data from the sensor. Default is 10s and 5 units
    
        **rs232para,0,10,5#**

    - Press <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) to Send command.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-english/gotrack365-el/send-command-sms/commands-4.jpg)

- Step 5: Save the configuration

    - Click on <span style="color:orange"> @</span> on the screen.
    - Select sample command: **Reset factory**. The command name will automatically appear on the screen.
    - Press <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) Send command to save and update configuration.

<span class="icon-left6">![Interface Web](/docs/assets/images/web-english/gotrack365-el/send-command-sms/commands-5.jpg)

- Step 6: Check sensor readings

    Wait a few minutes.

    - Click on <span style="color:orange"> @</span> on the screen.
    - Select sample command: **Read peripheral status**. The command name will automatically appear on the screen.
    - Press <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/send-sms.svg) to Send command.


- Step 7: Ask the device to send index updates to the web

    <span class="icon-left5">![Interface Web](/docs/assets/images/web-english/gotrack365-el/send-command-sms/@.jpg)
    - When the sensor readings have been read on the device, but the value has not been updated on the web, the following command can be used to request the device to send the sensor readings immediately.
    
        Enter the following command in the **Enter command** box:

        **pack,sensor#**
    
    
> If the device set **port 140.40**, the response will automatically update in the conversation. <br>
If the port is not set above, you will have to click on the icon <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/icons8-refresh.svg) to refresh the data.