



# **Deduction - Postman collection**

A Postman collection for Onboarding an employee in ADP Workforce Now.

Postman is a GUI REST client. By importing the collections you can explore our APIs and get a better understanding of the requests and responses.

Full API documentation can be found at [General Deduction RUN Guide](https://developers.adp.com/services/elasticsearch/articles/guides/c25aac4903f6323ab867f141f23968c7f0d3bcd8/doc/DeductionInstructionsAPIGuide-RUN.pdf).

## Getting Started

To get started with the Postman collections you will need to download the Postman tool from getpostman.com/postman.

With Postman installed, you can clone this repository or download the individual files. You can then import the files into Postman and start making your requests.

The collection consists of a POST ACCESS TOKEN CALL, this call consists of two headers, **Client_ID** and **Client_Secret** you need to request the details from your ADP representative who will be assisting you in this process. Once you make a successful call, you will be recieving an access token, this will be used in making the API call.    

The Feature call (aka API call) are configured to authenticate using a Authorization-Token variable that is sent with the request header. The value is stored in a variable called as **accessToken-wfn** and is automatically fetched once the user makes a successful ACCESS TOKEN CALL explained above.

## Important Note: 
1. First call should be token call so that it will be used in the feature.
2. Second call should be get payroll instruction API, so that it will fetch the values from the response for start, change & stop call.

## REST APIs

Our real-time REST APIs give you flexibility and customization to your needs.

## Collections include -

### Meta Call

This call will provide the values that are supported for the request payloads and will assist you in building the payload for the API.

### Happy Path - 200 Requests

Get Payroll instruction - This request will fetch all the active deductions for an worker.
General Deduction start - This request will add a deduction for an worker.
General Deduction change - This request will update the effective date or amount of an deduction.
General Deduction stop - This request will stop the deduction for an worker.

### Error Requests - 400 Series Requests

1. Invalid effective date - In the request payload passing a invalid effective date.
2. Invalid Item Id - In the request payload passing invalid item id.
3. Invalid Payroll File Number - In the request payload passing invalid payroll file number.
4. Invalid Payroll Agreement ID - In the request payload passing invalid agreement ID.

There is more help available for you, you can read [Make Your First API Call Using Postman](https://developers.adp.com/services/elasticsearch/articles/general/a20954ea9cb1ee5210dab5d9b3a3e5fc56f27953/doc/MakeYourFirstAPICallUsingPostman.pdf) and start your api journey.


