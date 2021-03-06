
.. include:: /API/APIHeadder.rst


Call Detail Record (CDR)
=========================

This API allows you to check your CDR for your account. 

:: 
 
 https://api.voicetel.com/cdr/[api_key]/
 
:: 
 
 https://api.voicetel.com/cdr/[start_timestamp]/[end_timestamp]/[api_key]/

**API Legend**

+---------------------+----------------------------------+---------------------------------------------+
|Property             |Description                       |Extra info                                   |
+=====================+==================================+=============================================+
|[api_key]            |Your API key                      |                                             |
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
|cdr                  |Data Container                    |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|id                   |Unique Identifier (UUID)          |Can be used to lookup a more detailed log    |
+---------------------+----------------------------------+---------------------------------------------+
|key[0]               |Account User Name                 |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|"cid"                |Originator Caller ID              |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|"dst"                |Destination Caller ID             |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|"ip"                 |Originator IP Address             |May be excluded if based on auth type        |
+---------------------+----------------------------------+---------------------------------------------+
|"dur"                |Call Duration in Seconds          |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|"nr"                 |Per Minute Rate                   |                                             |
+---------------------+----------------------------------+---------------------------------------------+
|"ba"                 |Billed Amount                     | If not billed for the call may be excluded  |
+---------------------+----------------------------------+---------------------------------------------+
|"cn"                 |Caller Id Name                    |(Optional)                                   |
+---------------------+----------------------------------+---------------------------------------------+


Example Output:

:: 
  
  {
  "status": "success",
  "cdr": [
    {
      "id": "UUID of the call",
      "key": [
        "User Name",
        "TimeStamp"
      ],
      "value": {
        "cid": "Caller ID",
        "dst": "Description",
        "ip": "IP address",
        "dur": "Duration in seconds",
        "nr": "Rate",
        "ba": "Amount Billed",
        "cn": "Caller ID Name",
      }
    }
  }
 

.. include:: /API/APIFooter.rst