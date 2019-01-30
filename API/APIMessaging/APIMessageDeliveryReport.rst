
.. include:: /API/APIHeadder.rst


Message Delivery Report
=========================

##This API will confirm delivery of massages to the end user.

:: 
 
 https://api.voicetel.com/dlr/[phone_number]/[api_key]/
 
:: 
 
 https://api.voicetel.com/dlr/[start_timestamp]/[end_timestamp]/[phone_number]/[api_key]/

**API Legend**

+---------------------+----------------------------------+---------------------------------------------+
|Property             |Description                       |Extra info                                   |
+=====================+==================================+=============================================+
|[api_key]            |Your API key                      |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|[phone_number]       |Number(DID) in NPANXXXXXX format  |Must be a VoiceTel Number(DID)               |
+---------------------+----------------------------------+---------------------------------------------+
|[start_timestamp]    |Start Unix Timestamp (Optional)   |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|[end_timestamp]      |End Unix Timestamp (Optional)     |                                             |
+---------------------+----------------------------------+---------------------------------------------+


**API Response**


+---------------------+----------------------------------+---------------------------------------------+
| Property            |REST Response                     |Extra info                                   |
+=====================+==================================+=============================================+
|status               |Success                           |If error check APIkey/Request                |
+---------------------+----------------------------------+---------------------------------------------+
|Message              |Detailed Response Message         |                                             |
+---------------------+----------------------------------+---------------------------------------------+


.. include:: /API/APIFooter.rst