>## Creating a device

The software provides at tool that allows you to configure a GPS tracking device to send data to your server without having to manually sends SMS messages.
Devices can be configured from the platform that are designed to receive SMS messages for IP, APN and port configurations. Trackers that require specific software to be configured cannot be set up using the GPS Device Activation tool.
It is also required to setup an SMS gateway in order to send SMS messages for configuration. Refer to the SMS Gateway section from the manual here.

To get started in creating and configuring a device, on the left panel under the "*Devices*" tab select the "*+*" icon.
 
<img src="_image/createdevices.png" alt="ajouter" width="auto">

A new menu will appear asking to fill out the name of the object and IMEI. The IMEI of the device can be found printed in a sticker on the device. Once the information is filled out, select the "*GPS device activation*" option and select the manufacturer of the device and the APN of the SIM data carrier.

<img src="_image/addautogps.png" alt="ajouter" width="auto">

***NOTE***: Make sure to enter the phone number of the SIM card with the country code in the *objects details -> Advanced* tab.

<img src="_image/avancedgps.png" alt="ajouter" width="auto">

If there are additional APN configurations that you would like to add or additional manufacturers with SMS commands, the settings are located in the Administrator panels "*Content*" tab.
This is only available in the White Label software.

<img src="_image/mapsevent.png" alt="ajouter" width="auto">



>## GPS device activation

The following menu displays all of the available manufacturers and models.
To add new commands for a different manufacturer, select the "*+*" icon in the right corner.
Or if an already existing manufacturers commands need to be added/adjusted, under "*Actions*" select the gear icon.

<img src="_image/activategps.png" alt="ajouter" width="auto">

Within the menu, enter the manufacturer and the model of the device.
For the SMS commands, select the "+" icon and type in the required command to configure the device. If the device requires more than one command to be configured and in a specific order, press the "+" button again and another line for the commands will be added. Add as many command lines as necessary for the device. The order in which the commands will be sent is from top to bottom.
When adding the commands to the list, instead of using the actual APN names and IP addresses, include the variables as the system automatically recognizes the APN configurations and the IP address.

***APN variables:***

* *% APNNAME%* - This is the APN name of the SIM data provider.
* *% APNUSERNAME%,% APNPASSWORD%* - These are usernames and passwords for the APN. If the data carrier does not require login credentials, these will be sent blank by the system.

***IP Address variable:***

* *% IP%* - The system automatically inputs Your server IP address into the configuration.

Once the details are entered, select "Save" and the recently added manufacturer with the commands will be added to the list.

<img src="_image/editsafe.png" alt="ajouter" width="auto">


>## APN configuration

All of the SIM data carriers with APN details are listed in the APN configuration menu. To add an additional provider, select the "*+*" icon on the right side of the menu. Or if the APN configurations need to be correct, under "*Actions*", select the gear icon.

<img src="_image/addapn.png" alt="ajouter" width="auto">

When creating a new APN configuration, a window will come up, prompting to enter the name of the data carrier, the APN name, APN username and password. The information has to be filled in according to the providers details.

<img src="_image/editapn.png" alt="ajouter" width="auto">

When the information is filled in, select "Save" and the data carrier with its APN details will be added to the list.






