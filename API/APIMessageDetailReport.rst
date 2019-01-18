
.. include:: APIHeadder.rst


Message Detail Report
=========================

With this API you will be able to check your inbound/outbound messages for a given phone number.You can also narrow down the range by providing a start and end Unix timestamp. 


Check all SMS for a given number.
:: 
 
 https://api.voicetel.com/mdr-sms/[phone_number]/[api_key]/
 
Check SMS for a given number with start and end timestamps.
:: 
 
 https://api.voicetel.com/mdr-sms/[start_timestamp]/[end_timestamp]/[phone_number]/[api_key]/
 
Check all MMS for a given number.
:: 
 
 https://api.voicetel.com/mdr-mms/[phone_number]/[api_key]/
 
Check MMS for a given number with start and end timestamps.
:: 
 
 https://api.voicetel.com/mdr-mms/[start_timestamp]/[end_timestamp]/[phone_number]/[api_key]/

**API Legend**

+---------------------+----------------------------------+---------------------------------------------+
|Property             |Description                       |Extra info                                   |
+=====================+==================================+=============================================+
|[api_key]            |Your API key                      |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|[phone_number]       |Number(DID) in NPANXXXXXX format  |Must be a VoiceTel Number(DID)               |
+---------------------+----------------------------------+---------------------------------------------+
|[end_timestamp]      |End Unix Timestamp (Optional)     |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|[start_timestamp]    |Start Unix Timestamp (Optional)   |                                             |
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