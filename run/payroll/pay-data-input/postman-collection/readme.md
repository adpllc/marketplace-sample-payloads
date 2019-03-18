

# **Pay data input - Postman collection**

A Postman collection for Adding and Replacing a pay data batch details for an employee in ADP Workforce Now.

Full API documentation can be found at [Pay Data Input API Guide-RUN](https://developers.adp.com/services/elasticsearch/articles/guides/ccbe89dcee99365523e0506ad7a09b7462be2d4c/doc/PayDataInputAPIGuide-RUN.pdf).

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

## /payroll/v1/pay-data-input
### Happy Path - 200 Requests
For Example

Retrieve the pay data batch details


## /events/payroll/v1/pay-data-input.add

### Happy Path - 200 Requests
For Example

1. Add a PayDataInput batch for anAssociate with pay Frequency as "Weekly"
2. Add a PayData batch with Different Earning codes for the same Associate
3. Add a pay data Batch with Regular Earning Code passing hours and amount.
4. Add a pay data Batch with OverTime Earning Code passing hours and Amount

### Error Requests - 4XX Series Requests
For Example

1. Add a pay data batch when there is an existing pay data file
2. Add a pay data batch when payrollGroupCode code is blank
3. Add a pay data batch when payrollGroupCode code is not valid
4. Add a pay data batch when hours for earning is negative value

## /events/payroll/v1/pay-data-input.replace

### Happy Path - 200 Requests
For Example

1. Replace a PayDataInput batch for anAssociate with pay Frequency as "Weekly"
2. Replace a PayData batch with Different Earning codes for the same Associate
3. Replace a pay data Batch with Regular Earning Code passing hours and amount.
4. Add a pay data Batch with OverTime Earning Code passing hours and Amount.
5. Replace a Pay data batch when using Department

### Error Requests - 4XX Series Requests
For Example

1. Replace the pay data batch when invalid item ID is passed
2. Replace a pay data batch when hours for earning is negative value
3. Replace a pay data batch when earning amount(rateValue) is negative
4. Replace a pay data batch when check number is not in following range(0-9)

There is more help available for you, you can read [Make Your First API Call Using Postman](https://developers.adp.com/services/elasticsearch/articles/general/a20954ea9cb1ee5210dab5d9b3a3e5fc56f27953/doc/MakeYourFirstAPICallUsingPostman.pdf) and start your api journey.
