---
category: section-mint-redemption
---

## MINT redemption

This API is for merchants to allows users to redeem a MINT ePin.

##### Parameters

|Parameter|Description|
|---|---|
|amount<br> *required*<br> **int**|The amount of money to pay|
|currency<br> *required*<br> **string**|[ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) currency code of the ePIN|
|epin<br> *required*<br> **array**|List of ePINs to redeem <br> Currently, it is only possible to redeem one ePin at a time.|
|app_key<br> *required*<br> **string**|The Project Key <br> Log in to your Merchant Account to get the Project Key in General Settings of the project|
|user_id<br> *required*<br> **string**|ID of the user in merchant's system|
