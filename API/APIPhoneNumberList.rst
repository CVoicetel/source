
.. include:: /API/APIHeadder.rst


Phone Number List
=========================

This API will pull a list of numbers for your account as well as routing destination.

:: 
 
 https://api.voicetel.com/numberList/[api_key]/

**API Legend**

+---------------------+----------------------------------+---------------------------------------------+
|Property             |Description                       |Extra info                                   |
+=====================+==================================+=============================================+
|[api_key]            |Your API key                      |                                             |
+---------------------+----------------------------------+---------------------------------------------+


**API Response**


+---------------------+----------------------------------+---------------------------------------------+
| Property            |REST Response                     |Extra info                                   |
+=====================+==================================+=============================================+
|status               |Success                           |If error check APIkey/Request                |
+---------------------+----------------------------------+---------------------------------------------+
|numbers              |Data Container                    |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|number               |Voicetel DID                      |Phone number in you account                  |
+---------------------+----------------------------------+---------------------------------------------+
|id                   |Unique ID for your gateway        |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|ip                   |Ware the calls are being routed   |                                             |
+---------------------+----------------------------------+---------------------------------------------+


Example Output:

:: 
 
 ##{
  "status": "success",
  "numbers": [
    {
      "number": "Phone Number 1",
      "id": "Gateway ID",
      "ip": "YourPBX.com:5080"
    },
    {
      "number": "Phone Number 2",
      "id": "Gateway ID2",
      "ip": "YourPBX2.com:5080"
    }
    ]
  }

.. include:: /API/APIFooter.rst