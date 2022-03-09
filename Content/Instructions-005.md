

There are two main API calls that allow access to Lab related Data.  There is the Details API call and the Result API call.  The Details API provides more details on a Lab including activity results whereas the Result API call focuses down on the result data of activities

>[**Details**](https://docs.skillable.com/lod/lod-api/lod-api-details.md) - Retrieves detailed information about a specified lab instance
>
>[**Result**](https://docs.skillable.com/lod/lod-api/lod-api-result.md) - Returns information about a particular lab instance result.

Having just completed a lab with scored activities let use thse two API Calls and see what they show and the differences.  We will start with the Results API as it returns less data.

- [] In Postman select the GET Result option from the Lab On Demand Postman Collection.  Notice this requires the single value for **labinstanceId**
- [] Overwritethe value with the Lab Instance ID recorded earlier: @lab.Variable(labinstanceID)
- [] Add the API key details to the Headers tab
- 

- [] Let the instructor know you have finished Lab 2.
