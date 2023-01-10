# ![PayDo](https://github.com/AnatoliyKulinich/paydo-api-doc/blob/master/images/logo.svg) **REST-like API Reference**

PayDo API is organized around [REST](http://en.wikipedia.org/wiki/Representational_State_Transfer).

PayDo API has predictable resource-oriented URLs, accepts [JSON](http://www.json.org/) request bodies, returns JSON responses, and uses standard HTTPS response codes.

Each request to PayDo API should have a `Content-Type` HTTPS header with `application/JSON` value.


## 
**PayDo integration options**



* [Hosted page](https://github.com/PaydoW/paydo-api-doc/blob/master/Integration/hostedPage.md) – a straightforward integration option using default PayDo checkout pages.
* [Direct integration](https://github.com/PaydoW/paydo-api-doc/blob/master/Integration/directIntegration.md) – bypassing the PayDo hosted page
* [Server-To-Server](https://github.com/PaydoW/paydo-api-doc/blob/master/Integration/serverToServer.md) – complex integration using PayDo API for users having a PCI DSS certificate

You can learn more about the difference between the above options here: [Difference description.](https://github.com/PaydoW/paydo-api-doc/blob/master/Integration/differenceDescription.md)


### **1. Payment methods**

With the help of these requests, you can get the methods available for payments.



* [Get available payment methods](https://github.com/PaydoW/paydo-api-doc/blob/master/Methods/getAvailablePaymentMethods.md)


### **2. Authentication**

Authentication is required to get access to the protected API actions.



* [Bearer authentication](https://github.com/PaydoW/paydo-api-doc/blob/master/Authentication/authentication.md)


### **3. API Response examples**

Description of API's response format with examples.



* [Successful response examples](https://github.com/PaydoW/paydo-api-doc/blob/master/Response/successResponse.md)
* [Failed responses](https://github.com/PaydoW/paydo-api-doc/blob/master/Response/failResponse.md)


### **4. Invoice**

An invoice is a basic entity in each payment system, a scheduled payment a customer makes toward the balance of goods or services.

Checkout transactions can be created only after invoice creation.



* [Payment methods](https://github.com/PaydoW/paydo-api-doc/blob/master/Checkout/getAvailablePaymentMethods.md)
* [Create invoice](https://github.com/PaydoW/paydo-api-doc/blob/master/Invoice/createInvoice.md)
* [Get invoice info](https://github.com/PaydoW/paydo-api-doc/blob/master/Invoice/getInvoice.md)


### **5. Checkout**

How to process payments.



* [Create checkout transaction](https://github.com/PaydoW/paydo-api-doc/blob/master/Transaction/createCheckoutTransaction.md)
* [Check transaction status](https://github.com/PaydoW/paydo-api-doc/blob/master/Checkout/checkTransactionStatus.md)
* [Card tokenization (*For Server-to-server integration only)](https://github.com/PaydoW/paydo-api-doc/blob/master/Checkout/createCardToken.md)
* [Get transaction info](https://github.com/PaydoW/paydo-api-doc/blob/master/Checkout/checkTransactionStatus.md)
* [IPN (instant payment notification)](https://github.com/PaydoW/paydo-api-doc/blob/master/Checkout/checkout.md#ipn-request-example)


### **6. Refund**

How to process refunds.



* [Create refund](https://github.com/PaydoW/paydo-api-doc/blob/master/Refund/createRefund.md)
* [Get merchant's refunds](https://github.com/PaydoW/paydo-api-doc/blob/master/Refund/getRefundList.md)
* [Get refund details](https://github.com/PaydoW/paydo-api-doc/blob/master/Refund/getRefund.md)


### **7. Wallet**

Wallet actions and payments.



* [Transfer money between wallets](https://github.com/PaydoW/paydo-api-doc/blob/master/Wallet/moveMoneyBetweenWalletsWithdrawal.md)
