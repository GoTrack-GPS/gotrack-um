# Fuel alert

To get a fuel alert, follow the steps below:

First, click on **Manage > Alerts - Schedule > Alert Rules**

<span style="display:block;text-align:left">![active device ](/docs/assets/images/web-english/notifications/alerts-rules.png)


### Create new

- Step 1: Click **Create New > Alert Type**.
- Step 2 :
 
  **2.1.** Select 1 from the list to generate an alert. A dialog box like the one below will appear

    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/add-fuel-alert.png)

    **Example** : **Sensor value min**

     - **Value** : Enter the minimum value (number of liters) to be alerted. If the tank capacity is below that value, an alert will be sent to let you know to refuel.
    - **Isloop** : Can enable/disable repeat. If repeat on, will choose how long to repeat / 1 time. Default is 5'/1 time for a alert violation.

    **2.2. Notification**
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/add-fuel-alert-notice.png)

    - **Name** : Enter the alert name.
    
    - **Text mess** : Notice what the problem is. Display accompanying when sending app/email alert
    
    - **Description** : Purpose, desire when creating this alert,...
    
    - **Activate** : Enable/disable the alert.

    - **SMS** : Enter a phone number in that box to add a phone number.
    
    - **Email** : Enter email in that box to add email.
    You can add 1 or more emails to send alerts about. (Email list separated by `,' or ';')

    - Tick the box <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square.svg) to enable setting / turn off **Get notified via mobile app**
    
        Or **Urgent Notice**

    - **Weekly : Choose the days and times** to receive notifications as you wish
    - **Date range**
      - **Always active**
      - **Active within** : Select a certain time period to receive that alert this week/this month,...
    
    **2.3. Device**
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/add-fuel-alert-device.png)

    - **Always select all devices** : On/Off applies the selected alert to all devices / 1 device number in that account.
    
    **2.4. Geofence**
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/add-fuel-alert-geofence.png)

    You can choose one of the following three options:
    - **Ignore** : Choose to receive all alerts. Both in and out geofence receive alerts.
    - **Out geofence**
    - **In geofence**

    **2.5. Sensor**
    
     <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/add-fuel-alert-sensor.png)


    - **Select all sensors** : On / Off applies to all sensors / 1 sensor in that account.

- Step 3: Click **Add** to complete the operation.


### Edit

* Step 1: Click <span class="icon-left svg-filter-info">![Ok](/docs/assets/images/web-interface/icon/SVG/edit.svg) to fix the alert.
* Step 2 :

    **2.1.** Select 1 from the list in the sensor to generate an alert. A dialog box like the one below will appear

    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/edit-alert-sensor.png)

    **Example** : **Sensor value min**

     - **Value** : Edit the minimum value (number of liters) to be alerted. If the tank capacity is below that value, an alert will be sent to let you know to refuel.
    - **Isloop** : Can enable/disable repeat. If repeat on, will choose how long to repeat / 1 time. Default is 5'/1 time for a alert violation.

    **2.2. Notification**
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/edit-alert-sensor-notice.png)

    - **Name** : Edit the alert name.
    
    - **Text mess** : Notice what the problem is. Display accompanying when sending app/email alert
    
    - **Description** : Purpose, desire when creating this alert,...
    
    - **Activate** : Enable/disable the alert.

    - **SMS** : Enter a phone number in that box to add a phone number.
    
    - **Email** : Enter email in that box to add email.
    You can add 1 or more emails to send alerts about. (Email list separated by `,' or ';')

    - Tick the box <span class="icon-left svg-filter-tick">![Ok](/docs/assets/images/web-interface/icon/SVG/check-square.svg) to enable setting / turn off **Get notified via mobile app**
    
        Or **Urgent Notice**

    - **Weekly : Choose the days and times** to receive notifications as you wish
    - **Date range**
      - **Always active**
      - **Active within** : Select a certain time period to receive that alert this week/this month,...
    
    **2.3. Device**
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/edit-alert-sensor-device.png)

    - **Always select all devices** : On/Off applies the selected alert to all devices / 1 device number in that account.
    
    **2.4. Geofence**
    
    <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/edit-alert-sensor-geofence.png)

    You can choose one of the following three options:
    - **Ignore** : Choose to receive all alerts. Both in and out geofence receive alerts.
    - **Out geofence**
    - **In geofence**
    
    **2.5. Sensor**
    
     <span style="display:block;text-align:left">![Interface manage acount](/docs/assets/images/web-english/notifications/edit-alert-sensor-sensor.png)

    - **Select all sensors** : On / Off applies to all sensors / 1 sensor in that account.
     
- Step 3: After finishing editing. Click **Save Changes** to complete the operation.


For more details, please refer to [here](modules/web-interface/notification/warning/)