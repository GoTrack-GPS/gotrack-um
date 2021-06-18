
# Dữ liệu lịch sử

### 1. Mô tả về API

- Lấy lịch sử dữ liệu trong khoảng thời gian truyền vào cho 1 phương tiện.

> Lưu ý : Khoảng thời gian truyền vào không quá 3 ngày.

### 2. URL 

```
[GET] {{host}}/api/v1/history-vehicle?apikey={apikey}&deviceId={deviceId}&timeFrom={timeFrom}&timeTo={timeTo}

```

### 3. Tham số


<table>  
    <tr>
        <td class="text-bold">Tên </td>
        <td class="text-bold">Loại</td> 
        <td class="text-bold">Trong </td>
        <td class="text-bold">Mô tả</td>  
    </tr>  
    <tr>
        <td >host </td>
        <td>string</td> 
        <td>path </td>
        <td></td> 
    </tr>
    <tr>
        <td >apikey </td>
        <td>string</td> 
        <td>path </td>
        <td>Do nhà cung cấp thiết bị hành trình cung cấp</td> 
        <tr>
        <td >deviceId </td>
        <td>number</td> 
        <td>path </td>
        <td>Id của thiết bị</td> 
    </tr>
    <tr>
        <td >timeFrom </td>
        <td>date</td> 
        <td>path </td>
        <td>thời gian bắt đầu format yyyy-MM-dd HH:mm:ss (timeFrom=2021-06-16 00:00:00)</td> 
    </tr>
    <tr>
        <td >timeTo </td>
        <td>date</td> 
        <td>path </td>
        <td>thời gian kết thúc format yyyy-MM-dd HH:mm:ss (timeTo=2021-06-16 23:59:59)</td> 
    </tr>
</table>


``` Không được lấy dữ liệu lịch sử quá 3 ngày```

### 4. Kết quả

#### 4.1. Lỗi
```
{
    "status": 400,
    "datetime": "2021-06-16 03:41:59",
    "message": "Key not empty.",
    "messageCode": "CLIENT__KEY_NOT_EMPTY",
    "result": null
}
```
```       
{
    "status": 400,
    "datetime": "2021-06-16 03:43:35",
    "message": "Device id not empty",
    "messageCode": "CLIENT__DEVICEID_NOT_EMPTY",
    "result": null
}
```
```
{
    "status": 400,
    "datetime": "2021-06-16 03:46:22",
    "message": "Time from not empty.",
    "messageCode": "CLIENT__TIME_FROM_NOT_EMPTY",
    "result": null
}
```
```        
{
    "status": 400,
    "datetime": "2021-06-16 03:48:25",
    "message": "Time to not empty.",
    "messageCode": "CLIENT__TIME_TO_NOT_EMPTY",
    "result": null
}
```
```
{
    "status": 401,
    "datetime": "2021-06-16 03:48:57",
    "message": "Key invalid.",
    "messageCode": "CLIENT__KEY_INVALID",
    "result": null
}
```
```
{
    "status": 403,
    "datetime": "2021-06-16 04:06:57",
    "message": "Does not permission get history of this device",
    "messageCode""CLIENT__DOES_NOT_PERMISSION_GET_HISTORY_THIS_DEVICE",
    "result": null
}
```
```
{
     "status": 400,
     "datetime": "2021-06-16 10:3:27",
     "message": "You can not get history data over duration of 3 days",
     "messageCode": "CLIENT__YOU_CAN_NOT_GET_hISTORY_TOO_3_DAY",
     "result": null
}
``` 

#### 4.2. Thành công
```
{
          "status": 200,
          "datetime": "2021-06-16 04:08:29",
          "message": "Get history successfully.",
          "messageCode": "CLIENT__GET_HISTORY_SUCCESS",
          "result": {
              "device": {
                  "imei": "1684070637",
                  "icon": {
                      "name": "direction"
                  },
                  "driver": {
                      "id": 0,
                      "name": "",
                      "driverCode": "",
                      "licenseNumber": "",
                      "phone": ""
                  },
                  "baseTemplate": [
                      {
                          "key": "input1",
                          "basic": false,
                          "value": "input1",
                          "active": true
                      },
                      {
                          "key": "input2",
                          "basic": false,
                          "value": "input2",
                          "active": true
                      },
                      {
                          "key": "input3",
                          "basic": false,
                          "value": "input3",
                          "active": false
                      },
                      {
                          "key": "input4",
                          "basic": false,
                          "value": "input4",
                          "active": false
                      },
                      {
                          "key": "input5",
                          "basic": false,
                          "value": "input5",
                          "active": false
                      },
                      {
                          "key": "input6",
                          "basic": false,
                          "value": "input6",
                          "active": false
                      },
                      {
                          "key": "input7",
                          "basic": false,
                          "value": "input7",
                          "active": false
                      },
                      {
                          "key": "input8",
                          "basic": false,
                          "value": "input8",
                          "active": false
                      },
                      {
                          "key": "input9",
                          "basic": false,
                          "value": "input9",
                          "active": false
                      },
                      {
                          "key": "input10",
                          "basic": false,
                          "value": "input10",
                          "active": false
                      },
                      {
                          "key": "input11",
                          "basic": false,
                          "value": "input11",
                          "active": false
                      },
                      {
                          "key": "input12",
                          "basic": false,
                          "value": "input12",
                          "active": false
                      },
                      {
                          "key": "input13",
                          "basic": false,
                          "value": "input13",
                          "active": false
                      },
                      {
                          "key": "input14",
                          "basic": false,
                          "value": "input14",
                          "active": false
                      },
                      {
                          "key": "input15",
                          "basic": false,
                          "value": "input15",
                          "active": false
                      },
                      {
                          "key": "odo1",
                          "basic": false,
                          "value": "odo1",
                          "active": false
                      },
                      {
                          "key": "odo2",
                          "basic": false,
                          "value": "odo2",
                          "active": false
                      },
                      {
                          "key": "odo3",
                          "basic": false,
                          "value": "odo3",
                          "active": false
                      },
                      {
                          "key": "odo4",
                          "basic": false,
                          "value": "odo4",
                          "active": false
                      },
                      {
                          "key": "odo5",
                          "basic": false,
                          "value": "odo5",
                          "active": false
                      }
                  ],
                  "sensorTemplate": [
                      {
                          "name": "demo23",
                          "id": 25,
                          "parameters": {
                              "max": 1000.0,
                              "min": 0.0,
                              "type": "linear",
                              "unit": "lit",
                              "round": 0,
                              "offset": 0,
                              "formula": "[value]",
                              "decrease": 20.0,
                              "increase": 20.0,
                              "typeSensor": "humid",
                              "show_on_map": false,
                              "parameter_name": "input1"
                          }
                      },
                      {
                          "name": "demoaccount",
                          "id": 63,
                          "parameters": {
                              "max": 1000.0,
                              "min": 0.0,
                              "type": "linear",
                              "unit": "l",
                              "round": 0,
                              "offset": 0,
                              "formula": "[value]/200",
                              "decrease": 20.0,
                              "increase": 20.0,
                              "typeSensor": "fuel",
                              "show_on_map": false,
                              "parameter_name": "input1"
                          }
                      }
                  ]
              },
              "routes": [
                  {
                      "timeFrom": "2021-06-13 17:00:00",
                      "timeEnd": "2021-06-14 16:59:59",
                      "routes": [
                          {
                              "type": "stop",
                              "start": {
                                  "updatetimeUTC": 1623603601,
                                  "powerVoltage": null,
                                  "battery": {
                                      "isAvailable": false,
                                      "voltage": null,
                                      "percent": null,
                                      "level": null,
                                      "isCharged": false
                                  },
                                  "lat": 20.979538333333334,
                                  "lng": 105.81824666666667,
                                  "speed": 0.0,
                                  "gsm": 5,
                                  "gps": 0,
                                  "direction": 161,
                                  "time": 1623603701,
                                  "address": "",
                                  "geofenceId": 0,
                                  "sensors": [
                                      {
                                          "id": 25,
                                          "value": 0
                                      },
                                      {
                                          "id": 63,
                                          "value": 0
                                      }
                                  ],
                                  "base": [],
                                  "distance": 0.0,
                                  "vin": ""
                              },
                              "end": {
                                  "updatetimeUTC": 1623626795,
                                  "powerVoltage": null,
                                  "battery": {
                                      "isAvailable": false,
                                      "voltage": null,
                                      "percent": null,
                                      "level": null,
                                      "isCharged": false
                                  },
                                  "lat": 20.979538333333334,
                                  "lng": 105.81824666666667,
                                  "speed": 0.0,
                                  "gsm": 20,
                                  "gps": 15,
                                  "direction": 0,
                                  "time": 1623626897,
                                  "address": "",
                                  "geofenceId": 0,
                                  "sensors": [
                                      {
                                          "id": 25,
                                          "value": 0
                                      },
                                      {
                                          "id": 63,
                                          "value": 0
                                      }
                                  ],
                                  "base": [],
                                  "distance": 0.0,
                                  "vin": ""
                              },
                              "points": [
                                  {
                                      "updatetimeUTC": 1623603601,
                                      "powerVoltage": null,
                                      "battery": {
                                          "isAvailable": false,
                                          "voltage": null,
                                          "percent": null,
                                          "level": null,
                                          "isCharged": false
                                      },
        								...
        								]
        							},
                          {
                              "type": "route",
                              "distance": 0.12081209117230389,
                              "start": {
                                  "updatetimeUTC": 1623626795,
                                  "powerVoltage": null,
                                  "battery": {
                                      "isAvailable": false,
                                      "voltage": null,
                                      "percent": null,
                                      "level": null,
                                      "isCharged": false
                                  },
                                  "lat": 20.979538333333334,
                                  "lng": 105.81824666666667,
                                  "speed": 0.0,
                                  "gsm": 20,
                                  "gps": 15,
                                  "direction": 0,
                                  "time": 1623626897,
                                  "address": "",
                                  "geofenceId": 0,
                                  "sensors": [
                                      {
                                          "id": 25,
                                          "value": 0
                                      },
                                      {
                                          "id": 63,
                                          "value": 0
                                      }
                                  ],
                                  "base": [],
                                  "distance": 0.0,
                                  "vin": ""
                              },
                              "end": {
                                  "updatetimeUTC": 1623626848,
                                  "powerVoltage": null,
                                  "battery": {
                                      "isAvailable": false,
                                      "voltage": null,
                                      "percent": null,
                                      "level": null,
                                      "isCharged": false
                                  },
                                  "lat": 20.979405,
                                  "lng": 105.818415,
                                  "speed": 0.0,
                                  "gsm": 15,
                                  "gps": 8,
                                  "direction": 164,
                                  "time": 1623626940,
                                  "address": "",
                                  "geofenceId": 0,
                                  "sensors": [
                                      {
                                          "id": 25,
                                          "value": 0
                                      },
                                      {
                                          "id": 63,
                                          "value": 0
                                      }
                                  ],
                                  "base": [],
                                  "distance": 0.0,
                                  "vin": ""
                              },
                              "points": [
                                  {
                                      "updatetimeUTC": 1623626795,
                                      "powerVoltage": null,
                                      "battery": {
                                          "isAvailable": false,
                                          "voltage": null,
                                          "percent": null,
                                          "level": null,
                                          "isCharged": false
                                      },
        								...
        								]
        							},
        							...
        					}
        				]
                  }
              ],
              "summary": {
                  "drivingTime": 2888,
                  "distance": 18.054889016180688,
                  "stopTime": 83254
              }
          }
        }
 ```
