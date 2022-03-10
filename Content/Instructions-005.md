

The Details API call allows access to all the Lab Instance related Data, this includes activity results.  There is two API calls listed in the documentation Result & Results.  Result is only there to maintain backward compatability for the API, the Results API call is to allow searching for Lab Instance IDs.

>[**Details**](https://docs.skillable.com/lod/lod-api/lod-api-details.md) - Retrieves detailed information about a specified lab instance

Having just completed a lab with scored activities let use the Details API Call and see what data it returns.

- [] In Postman select the **GET Details** API Call from the Lab On Demand Postman Collection.  Notice this requires the single value for **labinstanceId**
- [] Overwrite the value with the Lab Instance ID recorded earlier: +++@lab.Variable(labinstanceID1)+++
- [] Add the API key details to the Headers tab

| KEY | VALUE |
|-----|-------|
|+++api_key+++|+++@lab.Variable(api_key)+++|

- [] Press the **Send** button

The Details command returns lots of information about that Lab Instance as well as the activity data.  Spend some time reviewing the following and compare the date to the [**Details API**](https://docs.skillable.com/lod/lod-api/lod-api-details.md) documentation.  Specifically notice the following:

> The top few lines are about the Lab Profile and the User
> 
> The next section looks at Lab Duration both runtime, last activity time and save expiration time.  The time format is in Unix Epoch format.  Visit this website +++https://www.epochconverter.com/+++ and paste in one of the time values
>  
> The session section would show any saved sessions
> 
> The Notes section would show the notes added by the system during the Lab lifecycle
> 
> Copy the DetailsURL link and paste it into you local browser and compae the values above to what you see in LOD
> 
> The list then moves into summary exam data
> 
> Then lastly the specific data about each question

Later we will look at using this data for reporting.

- [] Save this API command as +++LDW - Details+++ in the **@lab.Variable(initials)-LDW Collection**

### Summary
In lab 2 you have launch a lab and review the lab status and avtivity output by using the LOD API

- [] Let the instructor know you have finished Lab 2.
