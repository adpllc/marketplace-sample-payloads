

# **Applicant Onboard - Post man collection**

A Postman collection for Onboarding an employee in ADP Workforce Now.

Full API documentation can be found at [Applicant Onboard WFN Guide](https://developers.adp.com/services/elasticsearch/articles/guides/82f633cbebcb730a22c4973082ed29542ed3bebc/doc/ApplicantOnboardAPIGuide-ADPWorkforceNow.pdf).

Postman is a GUI REST client. By importing the collections you can explore our APIs and get a better understanding of the requests and responses.

## Getting Started

To get started with the Postman collections you will need to download the Postman tool from getpostman.com/postman.

With Postman installed, you can clone this repository or download the individual files. You can then import the files into Postman and start making your requests.

The collection consists of a POST ACCESS TOKEN CALL, this call consists of two headers, **Client_ID** and **Client_Secret** you need to request the details from your ADP representative who will be assisting you in this process. Once you make a successful call, you will be recieving an access token, this will be used in making the API call.    

The Feature call (aka API call) are configured to authenticate using a Authorization-Token variable that is sent with the request header. The value is stored in a variable called as **accessToken-iat-wfn** and the value is stored automatically in the variable once the user makes a successful ACCESS TOKEN CALL explained above.

## REST APIs

Our real-time REST APIs give you flexibility and customization when verifying and enriching your contact data before it hits your database.

## Collections include -

### Meta Call

This call will provide the values that are supported for the request payloads and will assist you in building the payload for the API.


### Happy Path - 200 Requests

TEMPLATE -  Applicant Onboard - This request will result in a successful employee in work in progress using the template applicant onboard.

TEMPLATE -  HR Only - This request will result in a successful employee in work in progress using the template HR Only.

TEMPLATE -  HR + Payroll - This request will result in a successful employee in work in progress using the template HR + Payroll.

TEMPLATE -  HR + Time - This request will result in a successful employee in work in progress using the template HR + Time.


### Error Requests - 4XX Series Requests

TEMPLATE - QuickHire - http 400 Template Invalid - This Template is not supported by Work Force Know and is a limitation.

TEMPLATE - International Employees - http 400 Template Invalid - This Template is not supported by Work Force Know and is a limitation.

http 400 Applicant Onboard WFN - First Name as blank - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Applicant Onboard WFN - Last Name as blank - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Applicant Onboard WFN Expected Start Date as Blank - This is a mandatory field and if not passed in the request will result in a client error.

There is more help available for you, you can read [Make Your First API Call Using Postman](https://developers.adp.com/services/elasticsearch/articles/general/a20954ea9cb1ee5210dab5d9b3a3e5fc56f27953/doc/MakeYourFirstAPICallUsingPostman.pdf) and start your api journey.


