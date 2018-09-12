Data
===============
Data part is dedicated for data uploading, analysis and risk models preparation.

Data set
---------------
In this space data supplier can upload data and describe data structure for easier understanding.
Data set should not contain any sensitive or personal data.
File format should fit CSV standard "TODO: here".

CSV requirements
^^^^^^^^^^^^^^^^

* less than 10 Mb
* comma separated
* utf-8 encoding

Remote file access point
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
This field is for describing detailed steps how platform users will be able to access data file and download it.
Usually it is set when provided file is too large or contains other extension than .csv


Data set state
^^^^^^^^^^^^^^^^

* Waiting for approval - data set is currently under review by administrators
* Public - data set is visible for all platform visitors
* For logged in users - data set is visible for logged in users only
* Closed - data set is no longer relevant. No edit or new models submission allowed

Data set example
^^^^^^^^^^^^^^^^
::

    "DATE","REGION","DEVICEBRAND","DEVICEYEAR","BATTERYWEARLEVEL","ITEMID"
    "2017-09-21 16:29:50","unknown","asus","2016","100","bf2405968e460a53"
    "2017-09-22 9:35:15","unknown","meizu","2017","90","1002215a3478a570"
    "2017-09-22 20:36:15","unknown","pantech","2014","90","93e2b97de177ed99"
    "2017-09-23 18:12:20","unknown","lge","2014","90","2d3b8a37258d60e6"
    "2017-09-24 7:33:00","unknown","samsung","2016","90","6f45fb11f3c702d9"
    "2017-09-24 8:57:26","unknown","huawei","2017","0","1008b1d08d372006"
    "2017-09-24 13:17:10","unknown","explay","2014","90","4332da77a0e1f4d2"
    "2017-09-24 13:39:48","unknown","samsung","2017","90","3e2d1c3656ab5cc0"
    "2017-09-25 1:03:56","unknown","samsung","2014","90","928abd57acf557fa"

Each data set can be commented by logged in users.

Data models
-----------
Data model is insurance risk model which was made from data set. 
With data model user align risk for insurance product.
"Base premium" value is value from where risk multipliers begins.
For more precise models user can create up to 10 risk tables.

Each Data model can be up-voted. 

Model with highest vote will be implemented into insurance product and owner will get reward.

Data model example
^^^^^^^^^^^^^^^^^^^
Android Phone battery Insurance:  

Base premium: 2 ETH

+--------------+------------+
| DEVICEBRAND  | Multiplier |
+--------------+------------+
| asus         | 1          |
+--------------+------------+
| meizu        | 1          |
+--------------+------------+
| samsung      | 1          |
+--------------+------------+
| OTHERS       | 1.5        |
+--------------+------------+

+--------------+------------+
| DEVICEYEAR   | Multiplier |
+--------------+------------+
| < 2016       | 1.5        |
+--------------+------------+
| 2016         | 1.3        |
+--------------+------------+
| 2017         | 1.1        |
+--------------+------------+
| > 2017       | 1.3        |
+--------------+------------+

Example: 

If user has 2017 Samsung mobile device and wants to insure his battery, then "Risk premium" for him will be 2 * 1 * 1.1 = 2.2 ETH 

Insurance claim is valid and payout will happen if BATTERYWEARLEVEL is lower than 90.
