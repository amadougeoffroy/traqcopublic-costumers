>## Tools: overview

Tools are used to create alerts/notifications, geofences, POI's, send commands to GPS trackers, generate reports and many more.

<img src="_image/vuedensemble.png" alt="vuedensemble" width="auto">


>## Tools: Alerts

To create an alert choose "**Alerts**" in "**Tools**" menu on the main map window and press "*Add alert*" button (blue "*+*" symbol icon) on alerts panel.

<img src="_image/creeroutils.png" alt="creeroutils" width="auto">
<img src="_image/creeroutils2.png" alt="creeroutils" width="auto">

A new panel window will be opened. Start creating an alert by filling required information.  

<img src="_image/addalertes.png" alt="addalertes" width="auto">


>#### Devices

Enter alert name (required) and select objects (required) for which alert will generate.

<img src="_image/adddispositif.png" alt="adddispositif" width="auto">

>#### Type

Select alert type from the list. There are 7 types described as follows.

<img src="_image/typealerte.png" alt="typealerte" width="auto">

***Overspeed*** - this alert will generate when objects overspeed the value entered.

<img src="_image/Overspeed.png" alt="Overspeed" width="auto">

***Stop duration*** - this alert will generate when object is not moving for defined time in minutes.

<img src="_image/stopduration.png" alt="stopduration" width="auto">

***Driver change*** - this alert will generate when driver on object changes from selected drivers in the list.

<img src="_image/changepilote.png" alt="changepilote" width="auto">

***Geofence In*** - this alert will generate when object travels into geofence.

<img src="_image/geofencingadd.png" alt="geofencingadd" width="auto">

***Geofence Out*** - this alert will generate when object travels out of geofence.

<img src="_image/geofencingout.png" alt="geofencingout" width="auto">

***Geofence In / Out*** - this alert will generate when object travels in or out of geofence. Note that when selecting "*Geofence In*", "*Geofence out*" or "*Geofence In/Out*" alert types, "*Geofencing*" tab will be disabled.

<img src="_image/geoinout.png" alt="geoinout" width="auto">

***Custom events*** - this alert will generate when user created custom or system wide events are generated.

<img src="_image/personevents.png" alt="personevents" width="auto">

>#### Geofencing

Select geofences that will generate alert when object will be moving inside or outside geofence. This will work together with other type of alerts. For example it will generate overspeed alert only when moving inside or outside geofence.

<img src="_image/addalertgeofencing.png" alt="addalertgeofencing" width="auto">

>#### Schedule

Select when alert will be active. Press the mouse and paint on the calendar table. One table item is 15 minutes. Exact time stamp can be seen by hovering over the item with a mouse.

<img src="_image/addalerteprogramme.png" alt="addalerteprogramme" width="auto">

>#### Notifications

Select which notifications a user will get when alert generates.

There are sound notification that makes sound on web browser once alert generates.

Push notifications works also on mobile apps.

Email notification will send an email. 

SMS notifications will be sent to the numbers provided. SMS Gateway must be enabled to show this part of Notifications.

Webhook notification will use HTTP protocol to post data to given address.

<img src="_image/addnotif.png" alt="addnotif" width="auto">

>#### Command

Select command to activate when alert generates. Command will be sent to device trough GPRS network. 

<img src="_image/addcommand.png" alt="addcommand" width="auto">

Pressing "*Save*" button will finish alert creation steps and closes alert creation window.  


>## Tools: Geofencing


>#### Create a geofence

To create a new geofence, click *Tools->Geofencing->Add geofence*. Type in geofence name and select it's color, then click on the map to begin drawing geofence. When you finish drawing geofence, duoble click the last point and click *Save*.

<img src="_image/creercloture.png" alt="creercloture" width="auto">

Once geofence is created you can view them all on the list and edit anytime.

<img src="_image/addcloture2.png" alt="addcloture2" width="auto">

>#### Import and export

To import or export geofence click the button with a gear icon:

<img src="_image/importexport.png" alt="importexport" width="auto">

For export single, by groups, active and inactive geofences can be selected:

<img src="_image/importexport2.png" alt="importexport2" width="auto">

Export is saved in **.gexp** file.
 
For import only **.gexp** file can be used.  

>##### .gexp file structure

t is a simple text file that has following structure.

Example (single):


    {"groups": [], "geofences": [{"id": 1130, "group_id": 0, "name": "vn", "coordonnées": "[{\" lat \ ": 48.108348176168, \ "lng \": 14.284973144531}, {\ "lat \": 48.111099041065, \ "lng \": 14.403076171875}, {\ "lat \": 48.035855735787, \ "lng \": 14.400329589844}] "," polygon_color ": "# a34949"}]}

Format:

**" groups "** - name of the group geofence belongs. Emtpy [ ] means ungrouped.

**" geofences "** - liste des geofences. A l'intérieur, il faut remplir "**id**", "**group_id**", "**name**" et **"coordonnées"** - list of geofences. Inside it requires "id", "group_id", "name" and "coordinates" to be filled. "Coordinates" requires a list of "lat" and "lng" of coordinates to be filled.

**" polygon_color "** - color in html hex code.


>## Tools: Reports

>#### Main

To create a new report or schedule it, click *Tools->Reports* 

<img src="_image/rapportprincipale.png" alt="rapportprincipale" width="auto">

**Report**

* ***Title*** - report title/name
* ***Type*** - select report type
    * ***General information*** - report shows some basic information: top speed, average speed, consumed fuel, route length etc.
    * ***General information (merged)*** - general information displayed in a row.
    * ***Drives and stops*** - same information as general report but added: objects stops and driving information, like duration of intervals between stops, address where object stopped.
    * ***Travel sheet*** - displays coordinates and addresses of stops, fuel consumption, lenght between stops.
    * ***Overspeeds*** - speeding cases will be displayed in report as well as additional information such as excess time, how much speed has been exceeded.
    * ***Underspeeds*** - underspeeding cases will be displayed in the report.
    * ***Geofence in/out*** - entry/exit time in each zone and out zone, stay time in zone.
    * ***Events*** - events information: event name coordinates and address, time.
    * ***Service*** - service information.
    * ***Fuel level*** - information about fuel level changes.
    * ***Fuel fillings*** - object fuel fillings history.
    * ***Fuel thefts*** - object fuel thefts history.
* ***Format*** - select format that report will be generated: PDF (for viewving in Adobe Acrobat Reader), HTML (for viewing in browser), XLS (for viewing and editing in Microsoft Excel)
* ***Show addresses*** - near to location points addresses will be shown.
* ***Zones instead of addresses*** - instead of addresses zone names will be shown.
* ***Stops*** - set time of stops to eliminate traffic light stops.
* ***Speed limit (kph)*** - speed limit for Overspeed and Underspeed reports.

**Schedule**

* ***Daily*** - reports will be sent every day for previous day.
* ***Weekly*** - reports will be sent oncein a week, every Monday for previous week.
* ***Send to e-mail*** - enter e-mail addresses separated by comma to send reports to.

**Devices**

Select devices to create report.

**Geofences**

This allows to select zones whose details will be seen in report. Zone selection is available only if Report type Zone in/out is chosen.

**Time period**

* ***Filter*** - easy wayto set time period.
* ***Time from/ Time to*** - set time period of report.

>#### Generated reports

All generated reports can be visible in this tab. You can modify, regenerate and delete them.

<img src="_image/rapportgeneres.png" alt="rapportgeneres" width="auto">

>#### Scheduled reports logs

All scheduled generated reports. In case you did not received them via email, or don't need to, you can review them all here.

<img src="_image/journauxrapports.png" alt="journauxrapports" width="auto">


>## Tools: Send command

Commands can be sent via GPRS or SMS(sms gateway must be enabled (*Setup->SMS*)).

Type - if you select custom command, you will be able to send RAW gprs command to the device or select GPRS template you created in *Setup->GPRS Templates*.

If you want to see your specified gprs commands for selected device only, please go to *Objects->Edit->Advanced->Show* gprs templates only.

<img src="_image/envoicmd.png" alt="envoicmd" width="auto">

In order to send sms command to the device, sms gateway must be enabled (*Setup->SMS*).

<img src="_image/sendcmd.png" alt="sendcmd" width="auto">



>## Tools: Other

>#### Ruler

To check distance between 2 or more points, click *Tools->Ruler* and start clicking on the map.

>#### POI

POI - point of interest. These are the icons that you can put anywhere in the map and create label for it. POI import file format is **.KML**.

<img src="_image/autrepoi.png" alt="autrepoi" width="auto">

>#### Show point

With this tool you can see point on the map by entering coordinates or address.

>#### Show address

Shows an address by coordinates.


>## Tools: Camera

>#### Camera/Media tool

With this tool you can capture images from every GPS tracker, which has a camera attached. In the window you can see all trackers that have the cameras attached, you can also view the photos taken, select the camera via its id, if there are more than 1 camera attached to it, view the address and the map where the photo was taken.

It can be found through the main menu *Tools>Camera/Media*.

<img src="_image/appmedia.jpg" alt="appmedia" width="auto">

>#### Camera/DVR tool

If gps tracker does not support camera or you want to connect any other camera in the car, no matter which gps tracker you are using, this tool might be handy. Once ip camera or cameras are connected in the car, gps coordinates will be matched with camera by the closest available date and time.

To begin, please go to *Edit device->Cameras->Add camera*:

<img src="_image/addcamera.png" alt="addcamera" width="auto">

Type in any name you like and tick "*show widget*" if you want to see image in real time in widgets menu.
Once this is done, ftp username and password will be generated automatically for your camera. Please use those credentials to configure FTP settings in your IP camera so it can start sending images to the gps server:

<img src="_image/editcamera.png" alt="editcamera" width="auto">

Once FTP settings on cameras are set, you will begin to see images of them in real time. Also, you can preview history and photos along with device location:

<img src="_image/camerasvues.png" alt="camerasvues" width="auto">

In admin panel you can set how many days to keep device camera's images, in *Admin->Setup->Main* server settings.


>## Tools: Tasks

This tool allows you to create tasks, such as deliveries that can be assigned to objects using only the mobile GPS tracker application.

To create a task, navigate to *Tools -> Tasks*

<img src="_image/outilstaches.jpg" alt="outilstaches" width="auto">

A new window will appear that will ask you to fill out the necessary details for the task, such as the pickup and delivery addresses, the name of the task, priority, description and the object for the task to be assigned to.

(to add <img src="_image/.jpg" alt="outilstaches" width="auto">)

Once all of the information is entered, select "*Save*" and open the mobile GPS tracker application.
From the application, navigate to the Tasks tool and you will be greeted with the tasks assigned to object. To accept the task, hit "*Accept*".

<img src="_image/demotasks.jpg" alt="demotasks" width="auto">

Once the task is complete, you will be able to leave a signature, confirming that the task is complete.

<img src="_image/demotasks2.jpg" alt="demotasks2" width="auto">

To view the status of all the created tasks select the "*All tasks*" option from the web platforms Task feature.
You will also be able to view the signature of the completed deliveries.

<img src="_image/tachedelivres.png" alt="tachedelivres" width="auto">


>## Tools: Maintenance

With the maintenance tool, you can setup vehicle maintenance schedule to remind you of when the next vehicle service is due.
To open the maintenance tool, either select the "*Services*" tab within the objects details, or by enabling the "*Service*" widget in *Setup -> Widgets*, which appears at the bottom of the map when selecting and selecting the gear icon.

Accessing the maintenance tool via object's details:

<img src="_image/mantenaceedit.png" alt="mantenaceedit" width="auto">

Via "*Service*" widget by selecting the gear icon:

<img src="_image/maitenancevia.png" alt="maitenancevia" width="auto">

After opening the maintenance tool, the following screen will appear, displaying the currect schedules added. To create a new schedule, select "*Add service*".

<img src="_image/maintservices.png" alt="maintservices" width="auto">

Once selected, you will be prompted to enter the following information:

<img src="_image/addservices.png" alt="addservices" width="auto">

* ***Name:*** In this field you can add a name for the scheduled service.
* ***Expiration by*** - This is used to setup an expiration when the vehicle reaches a specific interval for one of the following options.

* Odometer  
* Engine hours
* Days 

* ***Interval:*** Setting a specific odometer, engine hours or day intervals when the vehicle is due for maintenance
* ***Last service:*** Used to enter a value when the vehicle was last serviced (odometer, engine hour or date value)
* ***Trigger event when left:*** A value to be entered if an alert should be triggered when there is a specific amount left before the service.
* ***Renew after expiration:*** Automatically renews the service schedule.
* ***Description:*** A brief description of the service.
* ***Email/Phone number:*** Required if an alert needs to be sent before the vehicle's service.

To view all of the created maintenance schedules, navigate to *Tools -> Maintenance*

<img src="_image/outils1.png" alt="outils1" width="auto">

<img src="_image/outils2.png" alt="outils2" width="auto">

>## Tools: Dashboard

The dashboard feature is used to display useful information in a more comprehensive way. It can be used to display device activity, events, device count (online/offline), task count and progress and the distance travelled by the devices.
It can opened manually or by setting up that the dashboard opens up everytime you open the map.

To enable the dashboard to open automatically and to enable which information to display, navigate to *Setup -> Dashboard*.

<img src="_image/outilsdashboard.png" alt="outilsdashboard" width="auto">

To open the dashboard manually, navigate to *Tools -> Dashboard*

<img src="_image/liendashboard.png" alt="liendashboard" width="auto">

An overview of the dashboard:

<img src="_image/dashboard.png" alt="dashboard" width="auto">

>## Tools: Sharing

The Sharing tool is used to create a shareable link to track GPS objects without having to login to the web platform.
To access the Sharing tool menu, navigate to *Tools -> Sharing*.

<img src="_image/outilspartage.png" alt="outilspartage" width="auto">

Once opened, you will be greeted with the following menu:

<img src="_image/partages.png" alt="partages" width="auto">

To created a shareable link, select the devices from the list that you'd like to be displayed in the map for others to see.
There are 3 options for durations:

* ***None*** - The link will last indefinetaly until it is deleted.
* ***Duration*** - The link will be accessible for a specific duration, which is up to 180 minutes.
* ***Date*** - A specific date can be set until the sharing link will expire.
    * ***Delete after expiration*** - this option is available when an expiration time/date is set for the link to delete it once it is expired.
Below the devices, there is an option to enter an email(s) to send a link as soon as it is created.

To view, edit and delete the created sharing links, navigate to "*Sharings*" from the top of the menu.

<img src="_image/sharing.png" alt="sharing" width="auto">






