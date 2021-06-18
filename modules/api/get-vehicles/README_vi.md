# Lấy danh sách phương tiện
### 1. Mô tả về API



### 2. URL 

```
[GET]  {{host}}api/v1/vehicles?apikey={apikey}
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
</table>

### 4. Kết quả

#### 4.1. Lỗi
```
{
    "status": 401,
    "datetime": "2021-06-12 03:45:29",
    "message": "Key invalid.",
    "messageCode": "CLIENT__KEY_INVALID",
    "result": null
}
```
```
{
    "status": 400,
    "datetime": "2021-06-12 03:46:16",
    "message": "Key not empty.",
    "messageCode": "CLIENT__KEY_NOT_EMPTY",
    "result": null
}
```

#### 4.2. Thành công
```
{
    status": 200,
    datetime": "2021-06-12 05:06:37",
    message": "Get list successfully.",
    messageCode": "CLIENT__GET_LIST_SUCCESS",
    result": [
       {
           "id": 848,
           "imei": "1684070637",
           "groupName": "demo",
           "groupId": 65,
           "simno": "0123456789",
           "userName": "demoaccount",
           "active": 1,
           "status": 4,
           "icon": "motorbike",
           "serviceExpire": "2021-08-27",
           "numberPlate": "30D11321",
           "machineCode": "SO MAY",
           "vinNumber": "123123123123",
           "frameNumber": "12125454",
           "name": "Vision - 102",
           "description": "desc",
           "createdAt": "2020-08-27 04:58:48",
           "createByUser": "demoaccount",
           "activeWarranty": 1,
           "warrantyActiveDate": "2020-08-27 04:59:05",
           "warrantyExpiredDate": "2021-08-27 04:59:05",
           "sortOrder": 0,
           "iconAdvancedJson": null,
           "updatedAt": "2021-05-26 11:09:21",
           "modifiedBy": "demoaccount",
           "coefficient": 1.2,
           "extensions": {
               "minSpeed": 1,
               "timeZone": 0,
               "timeoutGprs": 22,
               "isThirdParty": 0,
               "consumptionRate": 2.6,
               "minStopDuration": 600
           },
           "fwVersion": "",
           "typeName": "GT102",
           "simName": "VIETTEL",
           "driverName": "",
           "driverCode": "",
           "phoneDriver": "",
           "sensors": [
               {
                   "id": 25,
                   "deviceId": 848,
                   "name": "demo23",
                   "calculationType": "Linear",
                   "parameters": "{\"max\": 1000.0, \"min\": 0.0\"type\": \"linear\", \"unit\": \"lit\", \"round\"0, \"offset\": 0, \"formula\": \"[value]\"\"decrease\": 20.0, \"increase\": 20.0\"typeSensor\": \"humid\", \"show_on_map\": false\"parameter_name\": \"input1\"}",
                   "description": "",
                   "createBy": "demoaccount",
                   "createdAt": "2021-03-10 07:44:57",
                   "modifiedBy": "demoaccount",
                   "updatedAt": "2021-03-10 07:44:57",
                   "sortOrder": "0"
               },
               {
                   "id": 63,
                   "deviceId": 848,
                   "name": "vunv",
                   "calculationType": "Linear",
                   "parameters": "{\"max\": 1000.0, \"min\": 0.0\"type\": \"linear\", \"unit\": \"l\", \"round\": 0\"offset\": 0, \"formula\": \"[value]/200\"\"decrease\": 20.0, \"increase\": 20.0\"typeSensor\": \"fuel\", \"show_on_map\": false\"parameter_name\": \"input1\"}",
                   "description": "",
                   "createBy": "demoaccount",
                   "createdAt": "2021-06-08 09:38:49",
                   "modifiedBy": "demoaccount",
                   "updatedAt": "2021-06-08 09:38:49",
                   "sortOrder": "0"
               }
           ]
       }
    ]
}

 ```
```Note: id dùng để lấy trạng thái của xe, xem lại hành trình và báo cáo```