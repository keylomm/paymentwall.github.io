---
codeId: desktop-brick-charge-store-card-request
---
```
curl https://api.paymentwall.com/api/brick/charge \
-H "X-ApiKey: [YOUR_PRIVATE_KEY]" \
-d "token=[PERMANENT_TOKEN]" \
-d "amount=9.99" \
-d "currency=USD" \
-d "email=user@host.com" \
-d "fingerprint=[FINGERPRINT_BY_BRICK.JS]" \
-d "description=TestItem"
```