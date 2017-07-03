---
id: sandbox-pingback-tool
title: Pingback Tool
sectionid: docs
permalink: sandbox/pingback-tool
---

# Test Pingback Tool

Test Pingback tool is available for you to test how pingbacks work.

This tool is available in the Settings section of your Project once you set up the Pingback URL or Pingback Email:

<div class="docs-img">
    <img src="https://api.paymentwall.com/content/design/files/developers/documentation/apis/pingback/pw_pingback_url(1).png">
</div>

You can send a test pingback and provide your own values for every parameter for debug purposes.

<div class="docs-img">
    <img src="https://api.paymentwall.com/content/design/files/developers/documentation/apis/pingback/pw_test_pingback_2.png">
</div>

As a result of sending the Pingback you will see if Paymentwall received a successful response or not, as well as debug information about signature calculation.

<div class="docs-img">
    <img src="https://api.paymentwall.com/content/design/files/developers/documentation/apis/pingback/pw_test_pingback_success_2.png">
</div>

| **Type** | **Reason** | **API** | **Action needed** |
| 0 | Payment confirmation | Digital Goods / Brick | Deliver product to customer |
| 1 | Payment confirmation | Virtual Currency | Deliver virtual currency amount to customer |
| 2 | Refund/Chargeback | Digital Goods / Brick | Cancel product / virtual currency amount from customer's account |
| 200 | Risk status pending | Brick | Wait for approval/decline of transaction |
| 201 | Risk status approved | Brick | 	Deliver product to customer, transaction accepted |
| 202 | Risk status declined | Brick | Do not deliver product to customer, transaction blocked |
