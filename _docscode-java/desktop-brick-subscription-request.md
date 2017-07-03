---
codeId: desktop-brick-subscription-request
---
```java
Config.getInstance().setPublicKey("YOUR_APPLICATION_KEY");
Config.getInstance().setPrivateKey("YOUR_SECRET_KEY");

LinkedHashMap<String, String> subscriptionmap = new LinkedHashMap<String, String>();

subscriptionmap.put("token", request.getParameter("brick_token"));
subscriptionmap.put("email", request.getParameter("email"));
subscriptionmap.put("currency", "USD");
subscriptionmap.put("amount", "9.99");
subscriptionmap.put("description", "YOUR-DESCRIPTION");
subscriptionmap.put("fingerprint", request.getParameter("brick_fingerprint"));
subscriptionmap.put("plan", "YOUR-PRODUCT-ID");
subscriptionmap.put("period", "week");
subscriptionmap.put("period_duration", "1");

Subscription subscription = new Subscription();
subscription = (Subscription) subscription.create(subscriptionmap);
```