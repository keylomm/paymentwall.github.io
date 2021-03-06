---
category: section-tools-payment-systems
---

Request endpoint

```
GET https://api.paymentwall.com/api/payment-systems/
```

Request example
```
curl https://api.paymentwall.com/api/payment-systems/ \
-d "key=[YOUR_PROJECT_API_KEY]" \
-d "country_code=RU" \
-d "sign_version=2" \
-d "sign=[SIGNATURE]" \
```

Response:

```json
[
  {
    "id":"paypal",
    "name":"PayPal",
    "new_window":true,
    "img_url":"https:\/\/api.paymentwall.com\/images\/ps_logos\/pm_paypal.png",
    "img_class":"paypal",
    "ps_type_id":4
   },
   {
    "id":"alipay",
    "name":"AliPay",
    "new_window":true,
    "img_url":"https:\/\/api.paymentwall.com\/images\/ps_logos\/pm_alipay.png",
    "img_class":"alipay",
    "ps_type_id":4
   },
   {
    "id":"neosurf",
    "name":"Neosurf",
    "new_window":false,
    "img_url":"https:\/\/api.paymentwall.com\/images\/ps_logos\/pm_neosurf.png",
    "img_class":"neosurf",
    "ps_type_id":3
   },
   {
    "id":"mobiamo",
    "name":"Mobiamo",
    "new_window":false,
    "img_url":"https:\/\/api.paymentwall.com\/images\/ps_logos\/pm_mobiamo.png",
    "img_class":"mobiamo",
    "ps_type_id":5
   },
   {
    "id":"mint",
    "name":"MINT",
    "new_window":false,
    "img_url":"https:\/\/api.paymentwall.com\/images\/ps_logos\/pm_mint.png",
    "img_class":"mint",
    "ps_type_id":3
   }
]
```