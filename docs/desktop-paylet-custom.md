---
id: desktop-paylet-custom
title: Custom Price
sectionid: docs
permalink: paylet/custom-price
---

# Custom Price

Custom Price means that you are sending your products details through [our API](/apis#section-paylet-custom), and not storing it in Paymentwall side.

Here is a sample using Paylet widget.

<div class="docs-iframe" style="text-align: center;">
	<iframe src="https://api.paymentwall.com/api/subscription/?key=cd36b8635c7296dad972a239142c4b84&uid=user40012&widget=pw_1&amount=0.99&currencyCode=USD&ag_name=Gold+Membership&ag_type=fixed&ag_external_id=pw_t_2017051900001&sign_version=2&sign=0802bcbf5754b056458d4036fca74d24"></iframe>
</div>

> Make sure your project is configured as **Digital Goods API** in order to use Custom Price.

## Features

There will be only one product in our widget while using Custom Price as it doesn't have the products selection step, which means you need to create it by your own in your application. 

You can also build [deep-linked payment system](/paylet/widget/reference#deep-linked-payment-system) by using Custom Price for better payment experience. 

> See [widget reference](/paylet/widget/reference) for more features.

## Product type

The required parameters are different between onetime payments and subscription, please choose one according to your product type.

* [Onetime payments](/paylet/custom/onetime). Choose it if your product requires an instant payment for total amount.
* [Subscription](/paylet/custom/subscription)