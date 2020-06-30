>## Creating a device

<div class="row" style="text-align:left">
  <div class="col-md">

 To get started in creating and configuring a device, on the left panel under the "*Devices*" tab select the "*+*" icon.

</div>
<div class="col-md">
<img src="_image/createdevices.png" alt="ajouter" width="auto">
 </div>
</div>

A new menu will appear asking to fill out the name of the object and IMEI.
The IMEI of the device can be found printed in a sticker on the device.

<img src="_image/savedevice.png" alt="ajouter" width="auto">

Once the objects details are filled in, select "*Save*" and the created device will appear in the device list.

<img src="_image/devicesgroup.png" alt="ajouter" width="auto">


>## Configuring a device

Most GPS tracking devices are configurable using a series of SMS commands. The most important configurations in order for the tracking device to be acknowledged by the server are the IP address of the server you are using, the port of the device, APN name and username and password (if required by the data carrier) and time zone, which should be set to UTC-0.

To check which port your device uses, check our supported trackers page here. A list of IP addresses of our server can also be found in the supported trackers page. Make sure to refer to the user manual of your specific device for SMS configuration commands.
Below is an example of SMS commands used for Coban GT02A devices:

* ***Timezone#e0#*** - Timezone settings (UTC-0)
* ***Apn#APNname#APNusername#APNpassword#***  - APN details. If there are no credentials for the APN, can be left blank.
* ***Ip#138.201.205.20#6002#*** - IP address and port configurations. 
* ***Upload#10#*** - Data upload interval (seconds)

Once the device is configured, it will come up online.
Please allow up to 1 minute for the server to receive the first data packet from the device.

<img src="_image/savegroupe.png" alt="ajouter" width="auto">


