>## Available parameters

Global parameters are used in *Admin panel -> Setup -> Tracking ports*. Click edit near the port number and input parameter name and value below in the "Extra" section.
 
**List of available parameters:**
 
* ***ignoreFixTime / true or false*** - mostly used for Queclink devices, if you experience "Jumps" in history, please set this value to false.
* ***extended / true or false*** - for xexun protocol only
* ***can / true or false*** - for aplicom protocol only
* ***hbm / true or false*** - suntech protocol
* ***includeAdc / true or false*** - suntech protocol
* ***timeout / 1-9999*** - connection timeout value in seconds. Because sometimes there is no way to detect lost TCP connection, old connections stay in open state. On most systems there is a limit on number of open connection, so this leads to problems with establishing new connections when number of devices is high or devices data connections are unstable.
* ***timeoverride / true or false*** - once enabled, gps tracker time will be decoded the same as server time, this will fix the issue if tracker is always sending incorrect date and time.

