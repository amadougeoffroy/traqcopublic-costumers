>## Object popup

<img src="_image/fenetrecontaxtuelle.png" alt="fenetrecontaxtuelle" width="auto">

In the minimized popup window you can monitor basic information and sensors. Once you click "**Show more**", you will see all available information for this device including sensors, services, additional data. If you want ot check what parameters your device is sending, please visit sensor management section.

<img src="_image/appercurue.png" alt="appercurue" width="auto">

It is also possible to use "**street preview**" while monitoring your device. This window will refresh automatically once your device is moving, so you can "**street preview**" in real time.

>## Object quick tools

<img src="_image/outilsrapides.png" alt="outilsrapides" width="auto">

1. ***Show history*** - this will instantly show history of the object for most common selected period.
2. ***Follow*** - new window will appear where you will be able to monitor each object individually, you can open multiple windows at the same time.
3. ***Send command*** - quick access to send command to the device via gprs or sms.
4. ***Edit*** - edit device name, imei, accuracy, change icon, add services and more.

>## Edit - Main

<img src="_image/mainedit.png" alt="mainedit" width="auto">

To add device all is required is name and device imei or identifier. You can edit name and imei anytime.

>## Edit - Icons

<img src="_image/editicones.png" alt="editicones" width="auto">

***Icon type:***

* ***Arrow*** - arrow with direction and color(green, yellow, red) will be shown. This is default and recommended selection as it gives you the most control and information.
* ***Rotating icon*** - vehicle icon visible from the top will be show, it will rotate according to the direction.
* ***Icon*** - simple icon will be shown without direction and status.

***Icon type - Arrow. There are 4 states:***

* ***Moving*** - when device speed is higher than minimum speed defined in edit->accuracy->min. moving speed
* ***Stopped*** - when device speed is lower than minimum speed defined in edit->accuracy->min. moving speed
* ***Offline*** - if device is not sending information to the server 5 or more minnutes or is disconnected from the gps server
* ***Engine idle*** - for engine idle to be active, you need to add sensor for ignition on/off or engine on/off and then add that sensors in edit->accuracy->engine hours(switch from gps). Engine idle means that ignition/engine is on but device is not moving.

>## Edit - Advanced

<img src="_image/advanced.png" alt="advanced" width="auto">

In advanced section you can fill in optional information, assign device to the group(to create new group please go to *Setup->Groups->Add*).
 
* ***Show GPRS Tempaltes commands only*** - if you tick it, then only custom gprs commands will be showed for your device in *Tools->Send command*. GPRS templates can be created in Setup->GPRS Tempaltes
* ***Fuel measurement*** - if you do not have fuel sensors connected to your gps device, you can input measurements here so they will corespond in history and reports.
* ***Forward*** - Platform will copy and send raw device data to given IP and port in UDP or TCP connection.
* ***Time adjustment*** - this will manually adjust time individually for selected gps device. Used only in those cases, when you are unable to set timezone to UTC 0 for your device.

>## Edit - Sensors

Please check sensor managment page for detailed documentation.

>## Edit - Services

<img src="_image/servicesedit.png" alt="servicesedit" width="auto">

Services are used to monitor insurance, technical maintenance, oil change, car parts deprecation, etc.

>## Edit - Accuracy

<img src="_image/precisionedit.png" alt="precisionedit" width="auto">

* ***Engine hours*** - default selection is GPS, but if you have ignition or engine sensor connected to your gps tracker it is highly recommended to select it here. Once selected, if ignition is off you will not see unecessary history(like drifting), engine hours, distance, events like geofence or overspeed will not be triggered, therefore you will get the most accurate information including reports.
* ***Min. moving speed*** - if speed is below min. speed, moving will not be registered.
* ***Min. fuel difference to detect fuel fillings*** - if sensor value increases instantly by 10 units or more, fuel filling will be detected.
* ***Min. fuel difference to detect fuel thefts*** - if sensor value decreases instantly by 10 units or more, fuel theft will be detected.

​To prevent the platform from registering false movement when staying at one location and GPS points are not accurate "*Min. Moving speed*' value should be increased. Additionaly if device has an ignition sensor - adding it will stop platform registering location points when object ignition is off.

>## Edit - Tail

<img src="_image/editqueue.png" alt="editqueue" width="auto">

* ***Tail color*** - select color of the object tail
* ***Tail length*** - how long is the tail