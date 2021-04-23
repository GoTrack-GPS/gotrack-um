# Basic test and configuration guide
A few notes:

The device supports reading / configuring through 3 different channels: TCP / IP, COM-Terminal, SMS (structure and code are the same).

Important parameters such as IP / Port, ID, central phone will be protected (hereinafter referred to as locked device) after the device has been running continuously for 10 days, after this time the change of information. The above protected messages will be restricted and only made via central phone numbers or over the TCP / IP configuration channel to which the device is connected. (A message "No Permission @ ER #" will be returned when we change the parameters that are being protected from restricted channels).

Customer / Reseller should inform manufacturer about phone numbers that will be their own central number, so that the manufacturer can do this configuration before handing over to Customer / Reseller.

Please contact technical support for answers and best guidance.

### 1. Set up and check basic parameters
#### 1.1. IP / Port parameter

<table>
    <tr >
        <td rowspan="2"><b>Structure</b></td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Server,data,< ip/domain >,< port number >#</td>
        <td >Server,data#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td ><b>Example</b></td>
        <td >Server,data,125.212.235.145,13030#</td>
        <td >Server,data#</td>  
    </tr> 
    <tr >
        <td ><b>Feedback</b></td>
        <td >Server,data,125.212.235.145,13030#@OK#</td>
        <td >Server,data,125.212.235.145,13030@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3">* Updated after restarted by web <b>reset#</b></td>
    </tr> 
</table>

> Note: for the command set for this parameter to be successful, it should be as follows:
The device has not been configured locked (for checking, see item 2.10).
If the profile is locked, the phone number to be set up must be the central number. (For checking / setting, see section 1.9).
Perform the setup by sending commands from the server to which the device is connected.

#### 1.2. APN specifications

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Apn,< apn name needed to set > # </td>
        <td >apn #</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >apn,apn-name#</td>
        <td >apn #</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >apn,apn-name#@OK#</td>
        <td >apn,apn-name@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3">* Updated after restart by command <b>reset#</b></td>
    </tr> 
</table>


#### 1.3. Parameter APN-ROAMING


<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Apnex, < name apn when roaming needs setting ># </td>
        <td >Apnex#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Apnex,e-connect#</td>
        <td >Apnex#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Apnex,e-connect#@OK#</td>
        <td >Apnex,e-connect@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3">* Updated after restart by command <b>reset#</b></td>
    </tr> 
</table>

#### 1.4. Information transmission time

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Tim, < transmission time at run >, < on stop> # </td>
        <td >Tim#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Tim#,10,900#</td>
        <td >Tim#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Tim,10,900#@OK#</td>
        <td >Tim,30,900@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3"> * Default là 30,900 <br>
                         * Updated after responding OK and saved after restart by command  <b>reset#</b></td>
    </tr> 
</table>

#### 1.5. Timezone parameters

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Tzone, < time zone format ±HH.hh > # </td>
        <td >tzone#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Time zone: 9:30 -> “HH.hh” = 9 + 30/60 = 9.5 <br>
            Tzone,9.5#</td>
        <td >Tzone #</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Tzone,9.5#@OK#</td>
        <td >Tzone,9.5@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3"> * Default là +7.0 <br>
                         * Updated after responding OK and saved after restart by command  <b>reset#</b></td>
    </tr> 
</table>

#### 1.6. Speed parameters limit

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >speedth, < speed limit value > # </td>
        <td >speedth#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >speedth,120#</td>
        <td >speedth#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >speedth,120#@OK#</td>
        <td >speedth,120#@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3"> * Default là 120 <br>
                         * Updated after responding OK and saved after restart by command   <b>reset# </b>
        </td>
    </tr> 
</table>

#### 1.7. Buzzer buzzer setting

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Buzzer, < 0/1: disable/enable > #</td>
        <td >Buzzer#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Buzzer,1#</td>
        <td >Buzzer#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Buzzer,1#@OK#</td>
        <td >Buzzer,1#@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3"> * Default to turn on <br>
                         * Updated after responding OK and saved after restart by command<b>reset#</b>
        </td>
    </tr> 
</table>

#### 1.8. Set up digital input (ALT IO)

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >- For the ALT0 port <br> Altio,0, < ACC/AIR/SOS/DOO/BEN >,< positive level 0/1 > # <br>
            - For the ALT1 port <br> Altio,1, < ACC/AIR/SOS/DOO/BEN >,< positive level 0/1 > # </td>
        <td >Altio,0# <br>
            <br>
            Altio,1#
        </td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Altio,0,AIR,1#</td>
        <td >Altio,0 #</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Altio,0,AIR,1#@OK#</td>
        <td >Altio,0,AIR,1#@OK#</td>  
    </tr> 
     <tr >
        <td colspan="3"> * The default is AIR with ALT0 and SOS with ALT1 <br>
                         * Updated after responding OK and saved after restart by command  <b>reset#</b>
        </td>
    </tr> 
</table>

#### 1.9.	RS232 communication port setup (sensor connection)

##### 1.9.1. Connection establishment

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >- For the RS232_0 port  <br> Rs232,0, < sensor id >,< baudrate > # <br>
             - For the RS232_1 port <br> Rs232,1,< sensor id > ,< baudrate > # <br>
             -  sensor id:<br> 0/1/2 Turn off rs232 / FLS-Omnicom oil sensor / Soji oil sensor
        </td>  
        <td >Rs232,0# <br>
            <br>  <br> 
            Rs232,1#
        </td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Rs232,0,2,9600# (thiết lập cho cảm biến dầu Soji)</td>
        <td >Rs232,0#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >ARs232,0,2,9600#@OK#</td>
        <td >Rs232,0,2,9600#@OK#</td>  
    </tr> 
    <tr >
        <td colspan="3"> * Default is turn off <br>
                         * Updated after responding OK and saved after restart by command <b>reset#</b>
        </td>
    </tr> 
</table>

##### 1.9.2. Operation parameter setting

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
       <td >- For the RS232_0 port <br> 
                Rs232para,0, < sample time >, < trigger value ># <br> 
            - For the RS232_1 port <br>
                Rs232para,1, < sample time >, < trigger value ># <br>
            <b> sample time </b> : Sensor reading time, unit s, default 10s<br>
            <b> trigger value </b>: difference value between 2 last times to generate 1 sensor value update event, default is 5
        </td>  
        <td >Rs232para,0# <br>
            <br>  <br> 
            Rs232para,1#
        </td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Rs232para,0,20,10# <br> 
             <i>(set sensor sampling / reading frequency: 20s and update sensor value when difference is 10 or more units) </i>
</td>
        <td >Rs232para,0#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Rs232para,0,20,10#@OK#</td>
        <td >Rs232para,0,20,10#@OK#</td>  
    </tr> 
    <tr >
        <td colspan="3"> * Default is 10s and 5 units <br>
                         * Updated after responding OK and saved after restart by command<b>reset# </b> <br>
                         * To view sensor value sent to view command view, comm# <br>
        </td>
    </tr> 
</table>

##### 1.10.	Turn on / off digital output (Out0)

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Outputturn,0, < 0/1: tắt / bật > </td>  
        <td >Output,0#</td>  
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Outputturn,0,1#</td>
        <td >Outputturn,0#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Outputturn,0,1#@OK#</td>
        <td >Outputturn,0,1#@OK#</td>  
    </tr> 
    <tr >
        <td colspan="3"> * Default output is in the non-active state. <br>
                         * Instant updated and saved
        </td>
    </tr> 
</table>

- In addition, the device also supports generating a square pulse with Ton, Toff, adjustable cycles or a trigger (1 cycle pulse):

   * **Pulse**: outputpulse, 0, < Ton >, < Toff >, < number of cycles > #
   * **Trigger**: outputtrigger, 0, < Ton > #

##### 1.11.	Set up center phone number

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >Centralphone,< n >,< phone number > # <br>
            n: 0,1,2 (Support install 3 center numbers)
        </td>  
        <td >Centralphone,0# <br>
             Or <br>
             Centralphone,1# <br>
             Or <br>
             Centralphone,2# <br>
        </td>   
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Centralphone,0,0986026929#</td>
        <td >Centralphone,0#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Centralphone,0,0986026929#@OK#</td>
        <td >Centralphone,0,0986026929#@OK#</td>  
    </tr> 
    <tr >
        <td colspan="3"> * Updated after responding OK and saved after restart by command <b>reset# </b>
        </td>
    </tr> 
</table>

##### 1.12.	Set up a restart schedule

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Readc</td>  
    </tr> 
    <tr >
        <td >rebootsch, < n > ,< a > # <br>
            Perform schedule to reboot the device after “n” days at the right time at “a” time
             n = 0: this scheduling mode is disabled
        </td>  
        <td >rebootsch#</td>   
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >rebootsch,1,0#</td>
        <td >rebootsch#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >rebootsch,1,0#@OK#</td>
        <td >rebootsch,1,0#@OK#</td>  
    </tr> 
    <tr >
        <td colspan="3"> * This function is disabled by default <br>
                         * Updated after responding OK and saved after restart by command <b>reset# </b>
        </td>
    </tr> 
</table>

##### 1.13. Vibration sensor setting

<table>
    <tr >
        <td rowspan="2">Structure</td>
        <td >Establish</td>
        <td >Read</td>  
    </tr> 
    <tr >
        <td >motion,< 0/1: off / on>, <sensitivity index is a value less than 1>#</td>  
        <td >motion#</td>   
    </tr> 
     <tr >
        <td colspan="3"></td>
    </tr> 
     <tr >
        <td >Example</td>
        <td >Motion,1,0.05#</td>
        <td >motion#</td>  
    </tr> 
    <tr >
        <td >Feedback</td>
        <td >Motion,1,0.05#@OK#</td>
        <td >Motion,1,0.05#@OK#>  
    </tr> 
    <tr >
        <td colspan="3"> * Default is on and the sensitivity is 0.05 <br>
                         * Updated after responding OK and saved after restart by command<b>reset# </b>
        </td>
    </tr> 
</table>

-	Note: the smaller the sensitivity parameter value, the more sensitive it is to detect vibration and movement. Please take care while changing this parameter.

##### 1.14. Setting the power consumption balance (low voltage)

- The configuration software should be used for this.

### 2. Check active status
#### 2.1. Check device information


<table>
    <tr >
        <td>Commands</td>
        <td ><b>View, vehicleinfo#</b></td>
    </tr> 
    <tr >
        <td>Feedback content</td>
        <td >
       <b> vehi </b>, < License plate >, < distance: Km >, < speed >, < motion detection threshold >, < number of overspeed >, < time to maintain the current state at >, < total dwell time >, < velocity filtering: 0 / A or E is not used / filtered by ACC or Engine signals >. <br>
         <b> driv </b>, <ID card>, < driver's name >, < GPLX >, < start of journey >, < end of journey >, < tg continuous driving >, < total time driving > <br>
         <b> devi </b>, < device name >, < imei >, < hw-rev > , < Manuf-time >, < install-time >.
         <b> pwr </b>, < external power voltage >, < backup power voltage >
        </td>
    </tr> 
    <tr >
        <td>Example</td>
        <td >view,vehicleinfo, <br>
          <b>vehi</b> ,xxX-abc.de,0,0/10,0,9585,161,0 <br>
          <b>driv</b>,1dd46392500104e0 <br>
            ,LX_1dd46,gplx_1dd46,000000,000000,0,0 <br>
          <b>devi</b>,,S200,868183033819694,S2xx v1.0a,201020,201020 <br>
          <b>pwr</b>,19.39,0.00 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.2. Check overview

<table>
    <tr >
        <td>Commands</td>
        <td ><b>View, overview#</b></td>
    </tr> 
    <tr >
        <td>Feedback content</td>
        <td >
        <b> < device name > </b>, < imei >, < fw version >, < 0/1: the device is unlocked / locked >, < number of days the device was active >, < time of starting Dynamic DDMMYYhhmmss >, < Processor temperature > <br>
         <b> nw </b>, < 0/1: not available / have GPRS >, < signal strength, maximum: 31 > <br>
         <b> gps </b>, < 0/4/6:  state OK / ERROR / sleeping>, < 0/1: no / with position pin >, < satellite number > <br>
         <b> sv </b>, < server ip >, < server port >, < 0/1: not yet / connected > <br>
         <b> pw </b>, < mode: 0: normal / 1: sleeping >, < external power voltage >, < backup power voltage >, < charging mode >, < charging status > <br >
        <b>ti</b>, < ddmmyy >-< hh:mm:ss >
        </td>
    </tr> 
    <tr >
        <td>Example</td>
        <td >view, overview, <br>
          <b>S200</b>, 868183033877510,1.000.01.000000.201201,0,240,021220094301,34.3C <br>
            <b>nw</b>,1,20 <br>
            <b>gps</b>,0,1,6 <br>
            <b>sv</b>,125.212.235.145,13030,1 <br>
            <b>pw</b>,0,12.17,0.00,2,0 <br>
            <b>ti</b>,7.00,041220-11:13:08 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.3. Check peripheral status

<table>
    <tr >
        <td>Commands</td>
        <td ><b>View,comm#</b></td>
    </tr> 
    <tr >
        <td>Feedback content</td>
        <td >
        <b> led </b>, < state >, < 4 led indicator status, from left to right: "Drive" - ​​"Memory" - "Mobile network" - "GPS" > <br>
        <b> gps </b>, < state >, < 0-No good, 1-Good >, < satellite number > <br>
        <b> cell </b>, < state >, 1,1,1,1,1, < signal strength >, < sv connection state / server login state: 0-bad, 1-good > <br>
        <b> buz </b>, < state>, < 0/1: no bip / playing beep > <br>
        <b> rfid </b>, < state >, < tag ID > <br>
        <b> Acce </b>, < state >, < x-axis >, < y-axis >, < z-axis >, < xyz-axis > <br>
        <b> rs0 </b>, < state >, < sensor id >, < state >, < sensor reading value > <br>
        <b> rs1 </b>, < state >, < sensor id >, < state >, < sensor reading value > <br>
        <b> acc </b>, < state >, < active level > <br>
        <b> eng </b>, < state >, < active level > <br>
        <b> AIR </b>, < state >, 1, +, < active level > <br>
        <b> SOS </b>, < state >, 3, +, < positive level > <br>
        <b> DO </b>, < state >, < active level > <br>
        <i>state </i>: <br>
        &emsp;&emsp;&emsp;&emsp;-	7: disabled / not in use <br>
        &emsp;&emsp;&emsp;&emsp;-	6: reset <br>
        &emsp;&emsp;&emsp;&emsp;-	5: pause temporarily <br>
        &emsp;&emsp;&emsp;&emsp;-	4: Cannot connect to processor <br>
        &emsp;&emsp;&emsp;&emsp;-	3: packet error <br>
        &emsp;&emsp;&emsp;&emsp;-	2: checksum error <br>
        &emsp;&emsp;&emsp;&emsp;-	1: sleeping <br>
        &emsp;&emsp;&emsp;&emsp;-	0: Good <br>
        <i> Positive level </i>: 0-Off / Close, 1-On / On <br>
         <i> Led Status </i>: 0-Off, 1-No Flashing, 2-Fast Flashing (Flashing Fast), 3-Long Flashing (Slow Flashing).
        </td>
    </tr> 
    <tr >
        <td>Example</td>
        <td >view,comm, <br>
          <b>led</b>, ,0,0133<br>
            <b>gps</b>,0,1,5 <br>
            <b>cell</b>, 0,1,1,1,1,1,20,1/1 <br>
            <b>buz</b>,0,0 <br>
            <b>rfid</b>,0,3030303030303030 <br>
            <b>Acce</b>,0,0.00,-0.02,1.00,1.00 <br>
            <b>rs0</b>,0,2,4,0 <br>
            <b>acc</b>,0,0 <br>
            <b>eng</b>,0,0 <br>
            <b>AIR</b>,0,1,+,0 <br>
            <b>SOS</b>,0,3,+,0 <br>
            <b>DO</b>,0,0 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.4.	Check mobile network connection information


<table>
    <tr >
        <td>Commands</td>
        <td ><b>View,network#</b></td>
    </tr> 
    <tr >
        <td>Example</td>
        <td >view,network, <br>
            <b>reg</b>,1,1,1,1,1 <br>
            <b> cid</b>,89840480000616669331 <br>
            <b>nw</b>, 0,0,"Mobifone",20 <br>
            <b>cb</b>,EGSM_MODE,ALL_BAND,20 <br>
            <b>apn</b>,m-wap,e-connect <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.5. Check server connection status

<table>
    <tr >
        <td>Commands</td>
        <td ><b>View,serverconn#</b></td>
    </tr> 
    <tr >
        <td>Example</td>
        <td > 
            View, serverconn,10.82.117.62[0] <br>
            0.asia.pool.ntp.org:123,0,105311,LOST <br>
            27.72.57.208:5555,1,104609,LOST <br>
            125.212.235.145:13030,*,102409,OK <br>
            ota.GoTrack.vn:8086,0,,LOST <br>
            ota.GoTrack.vn:1111,0,,LOST <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.6. Check traffic consumption

<table>
    <tr >
        <td>Commands</td>
        <td ><b>View, idatameter# </b><br>
        (Flow is calculated from 00h)
        </td>
    </tr> 
    <tr >
        <td>Example</td>
        <td > 
            view,idatameter, <br>
            <b>Send/Rev </b>: 30.98/0.64KB <br>
            0:112412,112418,48B,0P,112417,48B,7P <br>
            1:112240,112245,12B,0P,112246,37B,18P <br>
            2:102409,102414,38B,0P,112749,50B,697P <br>
            3:,,0B,0P,,0B,0P <br>
            4:,,0B,0P,,0B,0P <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.7. Check memory and storage information

<table>
    <tr >
        <td>Commands</td>
        <td ><b>View, diskinfo# </b></td>
    </tr> 
    <tr >
        <td>Feedback content</td>
        <td >view,diskinfo, <br>
        <b> disk </b>, < 0: good >, < available / total KB space > <br>
         <b> dat </b>, < data file name >, < KB size >, < 1: log mode enabled > <br>
         <b> bak </b>, < log transfer information: number of bytes transferred / loss >, < Byte size of file > <br>
         <b>> TCP-Stream </b>
          < FIFO message number >, < BYTE capacity and FIFO address > <br>
         Q_NO_PROTEC <br>
         < number of transmitted messages / total number of messages in FIFO >: < number of remaining BYTEs of FIFO >
         @ OK #
    </td>
    </tr> 
    <tr >
        <td>Example</td>
        <td >view,diskinfo, <b>disk </b>,0,2800.0/7640.0
            <b>dat </b>,201204.TXT,95065,0x1
            <b>bak</b>,0/0,0
            <b>>TCP-Stream</b>
            120Msg,4096B@0x200032f8
            Q_NO_PROTEC
            0/0:4096
            @OK#
    </td>
    <tr >
        <td colspan="2" > 
           * Log (also known as historical data) is displayed in bak and < number of transmitted messages / total number of messages in FIFO >. Perform the test when the device update new data is not found
             * Clear log to immediately update new data using the command <b> fsmclean,log# </b>
        </td>
    </tr> 
</table>


#### 2.8. Check the vehicle's power supply status

<table>
    <tr >
        <td>Commands</td>
        <td ><b>View, powerinfo#</b></td>
    </tr> 
    <tr >
        <td>Example</td>
        <td > 
            view,powerinfo, <b>Main </b>,12.18,1(12.40-36.00) <br>
             <b>Bak </b>,0.00,0%,1(3.20-4.20) <br>
             <b>SW </b>,0/1,505000/10,180000/3 <br>
            @OK#
        </td>
    </tr> 
</table>

#### 2.9. Get the position of the current vehicle

<table>
    <tr >
        <td>Commands</td>
        <td >View,map#</td>
    </tr> 
    <tr >
        <td>Example</td>
        <td > 
            View,map,http://maps.google.com/maps?q=N%2020%2059.618626%20E%20105%2047.236412 <br>
            @OK#     
        </td>
    </tr> 
</table>

#### 2.10.	Configuration protection status

<table>
    <tr >
        <td>Commands</td>
        <td colspan="2" ><b>lockerstat#</b></td>
    </tr> 
    <tr >
        <td rowspan="2">Example</td>
        <td >lockerstat,0@OK# </td>
        <td >The configuration is not protected</td>
    </tr> 
    <tr >
        <td>lockerstat,1@OK#</td>
        <td >Configuration is protected (device is locked)</td>
    </tr> 
</table>

### 3. Other processing commands

#### 3.1. Delete log

* Fsmclean,log#

#### 3.2. Restart the device

* reset#

#### 3.3. Instant news transmission

* Pack, < packet-name: location/status/sensor/heartbeat >#
* Example: Pack,location#

#### 3.4. Get the phone number on the device

* Cellularsms, < phone number receives sms from device >, < SMS content that the device will send >#
Cellularsms, 0986026929, hello#
