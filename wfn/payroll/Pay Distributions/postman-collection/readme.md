
# **Pay Distributions(Direct Deposit) - Postman collection**

A Postman collection for adding,updating and removing a direct deposit for an employee in ADP Workforce Now.

Full API documentation can be found at [Direct Deposit API Guide - ADP Workforce Now](https://developers.adp.com/services/elasticsearch/articles/guides/b2643bb55850f43f51e4ade943cc1715b6a69439/doc/DirectDepositAPIGuide-ADPWorkforceNow.pdf).

Postman is a GUI REST client. By importing the collections you can explore our APIs and get a better understanding of the requests and responses.

## Getting Started

To get started with the Postman collections you will need to download the Postman tool from getpostman.com/postman.

With Postman installed, you can clone this repository or download the individual files. You can then import the files into Postman and start making your requests.

The collection consists of a POST ACCESS TOKEN CALL, this call consists of two headers, **Client_ID** and **Client_Secret** you need to request the details from your ADP representative who will be assisting you in this process. Once you make a successful call, you will be recieving an access token, this will be used in making the API call.    

The Feature call (aka API call) are configured to authenticate using a Authorization-Token variable that is sent with the request header. The value is stored in a variable called as **accessToken-iat-wfn** and is automatically fetched once the user makes a successful ACCESS TOKEN CALL explained above.

## REST APIs

Our real-time REST APIs give you flexibility and customization to your needs.

## Collections include -

### Meta Call

This call will provide the values that are supported for the request payloads and will assist you in building the payload for the API.

## POST /events/payroll/v1/worker.pay-distribution.change

### Happy Path - 200 Requests
For example
 
1. Retrieve the direct deposit
2. Add a direct deposit for an Associate when there are no existing deposits. 
3. A user has a list of direct deposits.Update one of the direct deposit with Amount only, effective immediately.



### Error Requests - 4XX Series Requests
For example

1. Add a Direct Deposit with a routing number in the wrong format.
2. Add a Direct Deposit for an existing Deduction Code for an employee.
3. Add a Full Net Direct Deposit when there is existing "Full Net" Deposit


There is more help available for you, you can read [Make Your First API Call Using Postman](https://developers.adp.com/services/elasticsearch/articles/general/a20954ea9cb1ee5210dab5d9b3a3e5fc56f27953/doc/MakeYourFirstAPICallUsingPostman.pdf) and start your api journey.
