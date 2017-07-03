---
codeId: pingback-listener-vc
---
```c#
using Paymentwall;

Paymentwall_Base.setApiType(Paymentwall_Base.API_VC);
Paymentwall_Base.setAppKey("YOUR_PROJECT_KEY"); // available in your Paymentwall merchant area
Paymentwall_Base.setSecretKey("YOUR_SECRET_KEY"); // available in your Paymentwall merchant area


NameValueCollection parameters = Request.QueryString;
Paymentwall_Pingback pingback = new Paymentwall_Pingback(parameters, HttpContext.Current.Request.ServerVariables["REMOTE_ADDR"]);
if (pingback.validate())
{
    float virtualCurrency = float.Parse(pingback.getVirtualCurrencyAmount());
    if (pingback.isDeliverable())
    {
        // deliver the virtual currency
    } else 
    {
        // withdraw the virtual currency
    }
    Response.Write("OK"); // Paymentwall expects response to be OK, otherwise the pingback will be resent
}
else {
    Response.Write(pingback.getErrorSummary());
}
```