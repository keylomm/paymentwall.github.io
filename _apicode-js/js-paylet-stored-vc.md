---
category: section-paylet-stored-vc
---
Endpoint

```
GET https://api.paymentwall.com/api/ps/?
```

Sample Request
```javascript
var Paymentwall = require('paymentwall');
Paymentwall.Configure(
  Paymentwall.Base.API_VC,
  'YOUR_APPLICATION_KEY',
  'YOUR_SECRET_KEY'
);

var widget = new Paymentwall.Widget(
  'user40012', // uid
  'p10', // widget
  {	
  	'email': 'user@hostname.com',
  	'timestamp': 'current_timestamp',
  	'addtional_param_name': 'addtional_param_value'
  }
);
widget.getHtmlCode();
```