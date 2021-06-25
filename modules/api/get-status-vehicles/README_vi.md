# Trạng thái thiết bị

### 1. Mô tả về API

- Lấy danh sách phương tiện tùy chọn chứa thông tin trạng thái tức thời

### 2. URL 

```
[GET]   {{host}}/api/v1/tracking-vehicles?apikey={apikey}&vehiclePlates={vehiclePlates}
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
    </tr>
    <tr>
        <td >vehiclePlates </td>
        <td>string</td> 
        <td>path </td>
        <td>Biển số xe. <br> Ngăn cách nhau bằng dấu <b>,</b> (vehiclePlates=1,2,3,4)</td> 
    </tr>
</table>

  
### 4. Kết quả

#### 4.1. Lỗi

``` 
{
    "status": 400,
    "datetime": "2021-06-16 04:34:06",
    "message": "Key not empty.",
    "messageCode": "CLIENT__KEY_NOT_EMPTY",
    "result": null
}
```
```
{
    "status": 400,
    "datetime": "2021-06-16 04:34:17",
    "message": "Device id not empty",
    "messageCode": "CLIENT__DEVICEID_NOT_EMPTY",
    "result": null
}
```
```
{
    "status": 401,
    "datetime": "2021-06-16 04:39:32",
    "message": "Key invalid.",
    "messageCode": "CLIENT__KEY_INVALID",
    "result": null
}
```
```
{
    "status": 500,
    "datetime": "2021-06-16 08:38:30",
    "message": "Get status device fail.",
    "messageCode": "CLIENT__GET_STATUS_DEVICE_FAIL",
}
```

#### 4.2. Thành công
```
{
            "status": 200,
            "datetime": "2021-06-16 08:38:30",
            "message": "Get status device successfully.",
            "messageCode": "CLIENT__GET_STATUS_DEVICE_SUCCESS",
            "result": [
                {
                    "favorite": 0,
                    "type": 24,
                    "status": "lost_gprs",
                    "statusDuration": 1782609,
                    "sensors": [
                        {
                            "id": 63,
                            "name": "vunv",
                            "unit": "l",
                            "type": "fuel",
                            "value": 0,
                            "maxValue": 1000
                        },
                        {
                            "id": 25,
                            "name": "demo23",
                            "unit": "lit",
                            "type": "humid",
                            "value": 0,
                            "maxValue": 1000
                        }
                    ],
                    "groups": null,
                    "groupName": "demo",
                    "groupId": 65,
                    "activeDate": "2020-08-27 04:59:05",
                    "name": "Vision - 102",
                    "lat": 20.97954,
                    "lng": 105.81818,
                    "powerVoltage": 13.0,
                    "battery": {
                        "isAvailable": false,
                        "voltage": 0.0,
                        "percent": 100.0,
                        "level": 0,
                        "isCharged": false
                    },
                    "dayDistance": 0.0,
                    "drivingTime": 0.0,
                    "dayDrivingTime": 0.0,
                    "direction": 224,
                    "icon": {
                        "name": "direction"
                    },
                    "geofenceObj": {
                        "id": 938,
                        "name": "Home"
                    },
                    "geofence": "Home",
                    "timestampUTC": 1622050101,
                    "updatetimeUTC": 1622050102,
                    "address": "",
                    "speed": 0.0,
                    "id": 848,
                    "imei": "1684070637",
                    "numberPlate": "30D11321",
                    "frameNumber": "12125454",
                    "odometer": 0.0,
                    "odoEngine": 0,
                    "driver": null,
                    "expiredAt": "2021-08-27 00:00:00",
                    "gsm": {
                        "level": 25,
                        "signal": 1
                    },
                    "gps": 0,
                    "simno": "0123456789",
                    "basic": [
                        {
                            "value": 0,
                            "type": "ignition"
                        },
                        {
                            "value": 0,
                            "type": "door"
                        },
                        {
                            "value": 0,
                            "type": "air"
                        },
                        {
                            "value": 0,
                            "type": "engine"
                        },
                        {
                            "value": -1,
                            "type": "seatBelt"
                        }
                    ],
                    "govManagement": "Hà Nội",
                    "updatetimeGPS": 1622046938,
                    "defence": 0,
                    "fuelToday": 0.0,
                    "stopEngineTS": 0,
                    "photos": [],
                    "photoIds": [
                        37
                    ],
                    "timeLive": 4429780,
                    "driverInfo": null,
                    "fwVersion": "",
                    "ccid": null,
                    "simStatus": 1,
                    "VIN": ""
                }
            ]
        }

 ```
```Note: id dùng để lấy trạng thái của xe, xem lại hành trình và báo cáo```