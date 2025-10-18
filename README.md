******Update Notice:
The integration is currently behind schedule due to issues with the Open API endpoint.
The following request does not return a valid response:{
  "id": 1,
  "method": "Es.GetStatus",
  "params": {
    "id": 0
  }
}
Home Assistant – Marstek Venus E V3.0 Local API As a result, development and testing have been delayed until the API behaves as expecteAs

This repository is dedicated to a custom Home Assistant integration for the Marstek Venus E V3.0 home battery system.  
The integration communicates with the battery through the Local API over UDP, which can be activated via the Marstek mobile app.

Important:

* This integration does not use the RS485 port.  
* Once the Local API is enabled, the communication is functionally equivalent to RS485 (Modbus), but it works over your local network (LAN/WiFi).  
* This avoids the need for RS485 adapters, ESP boards, or extra cabling.  

Current Status

This project is still under development.  
The goal is to provide full support for reading battery data directly in Home Assistant, including integration with the Energy Dashboard.

API Activation (Required)

To use this integration in the future, you must first ensure that the Local API is enabled on your Marstek Venus E V3.0:

1. Open the Marstek app.  
2. Go to Feedback / Support.  
3. Request a firmware update (minimum V137 or newer).  
4. Ask support to activate the Local API for your device.  

Once enabled, a new menu item will appear in the app:  
Settings → Advanced Functions → Local API  
Here you can toggle the Local API and set the UDP port (default 30000).  

Example request message (max 500 characters)

Hello Marstek team, thank you for the firmware updates. Could you please activate the Local API for my Venus E V3.0 battery (S/N: XXXXX)? I would like to use the UDP Local API on port 30000 for integration with my smart home system. Best regards.

Note

This repository currently serves as a development base and documentation hub.  
As the integration evolves, installation and configuration details will be added.
