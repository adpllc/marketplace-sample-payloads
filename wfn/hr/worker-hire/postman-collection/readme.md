


# **Worker Hire- ADP Workforce Now**


A Postman collection for posting a new hire into ADP Workforce Now® (ADP WFN).  A success post request will result a new employee record. 

Full API documentation can be found at [Worker Hire WFN Guide](https://developers.adp.com/services/elasticsearch/articles/guides/03181eb5019d9a1c40a9631a0f04586184a4bcc2/doc/WorkerHireAPIGuide-ADPWorkforceNow.pdf)

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


### Happy Path - 200 Requests

Worker Hire- This request will result in a successful posting of a new hire.




### Error Requests - 4XX Series Requests


http 400 Worker Hire - Event reason code is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Government ID Value is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Government ID codeValue is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Family Name is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Given Name is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Legal Address Line 1 is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - City Name is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire countrySubdivisionLevel1 is empty - This is a mandatory field and if not passed in the request will result in a client error.


http 400 Worker Hire Postal Code is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Birth Date is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - Hire Date is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - payPeriodAmount codeValue is blank - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - payrollGroupCode is empty - This is a mandatory field and if not passed in the request will result in a client error.

http 400 Worker Hire - SSN Number not in correct format 675-43-3 - This is a mandatory field and if not passed in the request will result in a client error.


There is more help available for you, you can read [Make Your First API Call Using Postman](https://developers.adp.com/services/elasticsearch/articles/general/a20954ea9cb1ee5210dab5d9b3a3e5fc56f27953/doc/MakeYourFirstAPICallUsingPostman.pdf) and start your api journey.
