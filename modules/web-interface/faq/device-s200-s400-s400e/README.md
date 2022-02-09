# Device S200/S400

### Question 1

* Q : We want to connect the device to our server with IP / port: 115.14123.160 / 16868 and the data transmission frequency is 10 seconds, how to do it?

* A : We can change these parameters via SMS, as follows:

    * [Refer to 1.1](modules/integrated-devices/smc/s200/sms-command/#ip) and write the command: **server,data,125.212.235.144.13030#** send to the phone number in the device
    * [Refer to 1.3](modules/integrated-devices/smc/s200/sms-command/#apn-roaming) compose command **tim,10,900#** sent to the device's phone number
    * In order for the device to save and update new profiles, write reset # and send to the phone number in the device. The device will then need time to reboot.

### Question 2

* Q : Our vehicle runs across the 2-country border, our phone sim has registered international roaming, but when crossing the border of your country, it no longer sends data. So we have to deal with, how to overcome

* A : In this case, it is very likely that you have not performed the APN configuration additionally, you need to contact the operator or the telecommunications service provider you are using to ask about the APN every time. SIM performs ROAMING in your home country. After we have this information, we will follow the command in item [1.13](modules/integrated-devices/smc/s200/sms-command/#ring).

### Question 3

* Q : I want to turn off the buzzer sound, because it would be annoying for the rental customer to hear it

* A: We can refer to order [1.7](modules/integrated-devices/smc/s200/sms-command/#bip), you write an SMS as follows: **buzzer,0#** then send to the phone number in the device.

### Question 4

* Q: Why am I going back to my previous configuration when I change my configuration for only a while?

* A: To ensure that the configuration is stored and updated, after you have finished the configuration to change the desired information, you should send a restart command: **reset#**

### Question 5

* Q: I see on the monitoring software, my vehicle shows the status of transmitting logs. How does my car position updates instantly.

* A: Your device has lost connection with the server for some time in the past, causing trip data to accumulate in memory and it is currently being retransmitted. If that data is not important and can be erased, we can execute the delete command as follows: **fsmclean,log#** send to the phone number in the device. (see also [2.7](modules/integrated-devices/smc/s200/sms-command/#log))

### Question 6

* Q: I often go to work on the elevated ring road, when the car has just reached 80km / h, how can the device buzzer to overcome this case?

* A: In your case, it is very likely that the device is in a speed warning, if it is a private vehicle you can change the speed limit for the warning, for example the road allows. up to 90Km / h, you can reconfigure by texting SMS: **speedth,90#** to the phone number in the device.

### Question 7

* Q: When I have installed the oil sensor on port **rs232_0** in port **A** I want to check the oil level status or value at the field in case I cannot see through the computer?

* A: In this case, you can do as follows, compose SMS: view, comm # to the phone number of the device. The device will respond to an SMS with the following illustrations:

    In case the oil level is not raised (from 1 ÷ 4095), you should check:

    * Port configuration, sensor type. Refer to [1.9](modules/integrated-devices/smc/s200/sms-command/#sensor)
    * Check that the device's TX, RX and sensor are cross connected or not.