---
category: section-paylet-optional-parameter
---
## Optional Parameter

Optional parameters could be added as additional information for extra needs. 

##### Parameters

| Name | Description |
|:--|:--| 
|success_url<br> **string**| URL of the page where the end-user should be redirected to after the payment is complete. |
|failure_url<br> **string**| URL of the page where the end-user should be redirected to after the payment is failed. Only is used when there is no way to complete this payment with this method. For credit cards user is not redirected to this page as he can still correct the error by using another card.|
|ps<br> **string**| To specify one payment option which to display in the widget. Only for Paymentwall Uni(p2), Paymentwall Mobile(m2) widgets. Please refer [Payment system codes](/ps-codes) page to get the parameter values for each payment option. |
|pingback_url<br> **string**| Optional URL of pingback listener script where pingbacks should be sent. Overrides the default Pingback URL set up in Project Settings inside of merchant account. Takes effect only if activated for the merchant account per request by sending email to [devsupport@paymentwall.com](mailto:devsupport@paymentwall.com). |
|lang<br> **string**| Language code to override the default geo-targeted language of the widget. 2 letters. eg: en. See [language codes](/lang).|
|evaluation<br> **integer**|The value could be either 1 or 0. For test environment only.<br> If 1, everyone can see the content without being logged into the merchant account in the same browser session.|
|country_code <br> **string** | The length must be 2-character according to [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) code of the country. Overrides the default geological location of user. Requires widget signature.|