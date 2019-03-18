
# **Pay data input modify - Postman collection**

A Postman collection for creating a batch for an employee in ADP Workforce Now.

Full API documentation can be found at [Payroll Data Input API Guide - ADP Workforce Now](https://developers.adp.com/services/elasticsearch/articles/guides/2290c84affffb44938074db32d803471db31fd6b/doc/PayrollDataInputAPIGuide-ADPWorkforceNow.pdf).

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

## /events/payroll/v1/pay-data-input.modify
### Happy Path - 200 Requests
For Example

1. Add a pay data batch with different codes for Multiple associates for codedHoursEarningInputs.
2. Add a pay data batch with Hours for Regular Earning.
3. Add a pay data batch with Amount for Regular Earning.
4. Add a pay data batch with Hours for OverTime Earning Code.
5. Add a pay data batch with Amount for OverTime Earning Code.
6. Add a pay data batch with Temp Rate and Hours for Regular Earning.
7. Add a pay data batch with Temp Rate and Hours for OverTime Earning



### Error Requests - 4XX Series Requests
For Example

1. Add a pay data batch when the payroll cycle Status is not in Entering Payroll Information or Correcting Input.
2. When an invalid Company code is passed in the request.
3. When an invalid Associate Organization ID (AOID). This is AOID associated to the file number passed in the request.	
4. When Invalid payrollFileNumber is passed in the request.
5. When an invalid pay Number is passed in the request.


There is more help available for you, you can read [Make Your First API Call Using Postman](https://developers.adp.com/services/elasticsearch/articles/general/a20954ea9cb1ee5210dab5d9b3a3e5fc56f27953/doc/MakeYourFirstAPICallUsingPostman.pdf) and start your api journey.
