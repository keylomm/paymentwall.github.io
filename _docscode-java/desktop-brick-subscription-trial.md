---
codeId: desktop-brick-subscription-trial
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

subscriptionmap.put("trail[amount]", "0.5");
subscriptionmap.put("trail[currency]", "USD");
subscriptionmap.put("trail[period]", "day");
subscriptionmap.put("trail[period_duration]", "3");
Subscription subscription = new Subscription();
subscription = (Subscription) subscription.create(subscriptionmap);
```