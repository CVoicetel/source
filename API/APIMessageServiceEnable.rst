
.. include:: APIHeadder.rst


Messaging Enablement
=========================

This API enables a number to be used with SMS/MMS. You will also need to enable massaging services in your Portal>Settings>Messaging Services.

:: 
 
 https://api.voicetel.com/smsEnable/[number]/[api_key]/

**API Legend**

+---------------------+----------------------------------+---------------------------------------------+
|Property             |Description                       |Extra info                                   |
+=====================+==================================+=============================================+
|[api_key]            |Your API key                      |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|[number]             |Number in NPANXXXXXX format       |                                             |
+---------------------+----------------------------------+---------------------------------------------+

**API Response**


+---------------------+----------------------------------+---------------------------------------------+
| Property            |REST Response                     |Extra info                                   |
+=====================+==================================+=============================================+
|status               |Success                           |If error check APIkey/Request                |
+---------------------+----------------------------------+---------------------------------------------+
|Message              |Detailed Response Message         |                                             |
+---------------------+----------------------------------+---------------------------------------------+


.. include:: APIFooter.rst