# Configure to receive images sent from S200 / S400 devices

### 1. Wiring

* RX of MDVR -> TX of S200 / S400: Yellow
* TX of MDVR -> RX of S200 / S400: Blue

### 2. Configure on the device

- RS232 port
* rs232,0,9,115200 #
- Shooting frequency: 300 seconds
rs232para,0.300.0 #
- Server and image upload path:
* server,file,__ photos.gotrack365.com,80__# or * server,file,__125,212.235.150,9191 __#
* server,path,__/api/receive-photos__ #

* __reset #__