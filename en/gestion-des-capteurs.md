>## Add new sensor

To add new sensor (**engine on/off**, **acc on/off**, **battery**, **fuel tank**, **odometer**, **temperature**, **door open/close**, **GSM signal**, **GPS signal**, **sattelites**, **tachometer**, etc.) for your object, go to *Object->Edit object->Sensors->Add new sensor*. But before doing that, take a look below at the scheme, how parameters are sent from gps device and how they need to be **paired** with sensors.



<img src="_image/gestionaddcapteur.png" alt="ajouter" width="auto">

To check what parameters your gps tracker is sending, please go to *History->Select object->Show history->Data log*

*(At the top there are parameter names and below - parameter values)*

<img src="_image/gestionaddcapteur2.png" alt="ajouter" width="auto">

There are many parameter names like **"sat, adc1, io21..."** etc. So if you want to create an event for parameter **"sat"**, then you have to input sat in the parameter name field. This will pair event with parameter.

***Note:*** *some gps tracker's, like Coban GPS306 OBD, are sending parameter names that are easily recognisable(odometer, fuel, rpm, etc.), but others, like Teltonika are sending them like ioXXX. To know the meaning of parameter names like ioXXX, you need to check manufacturer's user manual/documentation or identify them manualy, for example, trigger some sensors and monitor parameters at the same time like doors open, fuel level, etc...*


>## ACC ON / OFF

<img src="_image/acconoff.png" alt="ajouter" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***ON value*** - please input parameter value to identify that acc was turned on. For example.: if parameter name is alarm: acc on, type in ***acc on***
* ***OFF value*** - please input parameter value to identify that acc was turned off. For example.: if parameter name is alarm: ***acc off***, type in ***acc off***
* ***Setflag*** - is used to detect single or few characters from parameter value. Example.: 12345 is parameter value and „***34***“ is the value you want to use, so setflag would be: ***3***(starting character), ***2***(ammount of characters), ***34***(value of parameter)“.


<img src="_image/acconoff2.png" alt="ajouter" width="auto">


>## Battery

<img src="_image/baterieadd.png" alt="ajouter" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor. Example: battery: 75 (visible in data log) must be selected as battery. In the exaple above "sat" is selected which means that you can use any type of sensors with ***any type*** of parameter.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***Show value by "Parameter value"*** - parameter value will be shown.
* ***Show value by "Min/Max values"*** - for example if full battery value is 5, minimum 0, please type in 5 in the max value field and 0 in the min value field, so it will automatically convert it to percentage values. For example.: if value is 5 - 100 will be show, if value is 4 - 75 will be show, if value is 0 - 0 will be seen.
* ***Show value by "Formula"*** - parameter value can be sent from gps tracker encoded and you have to use formula to calculate battery value. For example.: if value is 2850, then you can type in formula like "([value] x 3.3)/4096", for example: ([28501] x 3.3)/4096 = 22.96 %
* ***OFF value*** - please input parameter value to identify that acc was turned off. For example.: if parameter is alarm: acc off, type in ***acc off***



>## Doors Open/Close

<img src="_image/openclosedoors.png" alt="ajouter" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***ON value*** - please input parameter value to identify that acc was turned on. For example.: if parameter name is alarm: acc on, type in ***acc on***
* ***OFF value*** - please input parameter value to identify that acc was turned off. For example.: if parameter name is alarm: acc off, type in ***acc off***

>## Engine On/Off

<img src="_image/marchearret.png" alt="marchearret" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***ON value*** - please input parameter value to identify that acc was turned on. For example.: if parameter name is alarm: acc on, type in ***acc on***
* ***OFF value*** - please input parameter value to identify that acc was turned off. For example.: if parameter name is alarm: acc off, type in ***acc off***


>## Engine hours

<img src="_image/heuremoteur.png" alt="heuremoteur" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"

>## Fuel tank

<img src="_image/reservoirdessence.png" alt="reservoirdessence" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***Fuel tank name*** - any name like Petrol, Diesel etc.
* ***Parameters*** - for example if tacker is sending fuel in percentage value like 100 and your car's full tank is 40 liters, then type in 40 on the left side(full tank) and 100 on the right side(parameter value), so when tracker sends parameter value 50, you will see that your car's fuel tank is 20 liters or gallons.


>## Fuel tank with calibration

<img src="_image/reservoiretalonnage.png" alt="reservoiretalonnage" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
Sensor type - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***Fuel tank name*** - any name like Petrol, Diesel etc.
* ***Calibration*** - gps trackers can send fuel level in voltages or any other values, therefore calibration is needed. Above is example of parameter value and matching liters/gallons value. It is best to start calibration with full tank and check parameter value and then move on with empty fuel tank and check parameter value again.


>## GSM

<img src="_image/gsm.png" alt="gsm" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***Show value by "Min/Max values"*** - for example if full battery value is 5, minimum 0, please type in 5 in the max value field and 0 in the min value field, so it will automatically convert it to percentage values. For example.: if value is 5 - 100 will be show, if value is 4 - 75 will be show, if value is 0 - 0 will be seen.

>## Harsh acceleration and harsh braking

<img src="_image/accelerationbrutale.png" alt="accelerationbrutale" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Parameter value*** - value for detecting harsh acceleration or braking. Once values configured, you can then generate driver behavior report: *Tools->Reports->RAG*


>## Ignition ON/OFF

<img src="_image/allumage.png" alt="allumage" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***ON value*** - please input parameter value to identify that acc was turned on. For example.: if parameter name is alarm: acc on, type in acc on
* ***OFF value*** - please input parameter value to identify that acc was turned off. For example.: if parameter name is alarm: acc off, type in ***acc off***

>## Odometer (connected and virtual)

<img src="_image/odometre.png" alt="odometre" width="auto">
<img src="_image/odometre2.png" alt="odometre2" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example you can define km or mi
* ***Odometer*** - if you selected connected odometer, please pair it with parameter that is responsible for connected odometer value, otherwise please select Virtual Odometer.
* ***Forumula*** - value can be sent in meter, kilometers, miles, feets, etc., so using formula you can apply correct calculations.


>## Satellites

<img src="_image/satellite.png" alt="satellite" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"

>## Tachometer/RPM or temperature

<img src="_image/tachometre.png" alt="tachometre" width="auto">

* ***Sensor name*** - in this field you can write in any name you like. This name will appear as sensor name in object details panel when you click on the object.
* ***Sensor type*** - this is type of sensor, each sensor type has different parameters input options and behaviour.
* ***Parameter name*** - parameter names are identified automatically once gps tracker is connected to the platform, select the coresponding parameter that matches your sensor.
* ***Unit of measurement*** - this text will be showed near value, for example, if you define battery sensor, then you can type in % as unit of measurement, then you will see battery sensor like "battery: 25%"
* ***Forumula*** - using formula you can apply correct calculations.
