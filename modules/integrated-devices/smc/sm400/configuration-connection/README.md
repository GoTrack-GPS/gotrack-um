
# Configure to receive images sent from S200 / S400 devices

### 1. Wiring

* RX of MDVR -> TX of S200 / S400: Yellow
* TX of MDVR -> RX of S200 / S400: Blue

### 2. Configure on the device

- RS232 port

   **rs232,0,9,115200 #**

- Shooting frequency: 300 seconds

    **rs232para,0.300.0 #**

- Server and image upload path:

    **server,file,photos.gotrack365.com,80#** 

    **server,path,/api/receive-photos#**

    **reset#**