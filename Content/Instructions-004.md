
# 004 - Lets launch a Lab

### In this activity you will launch a lab and then complete the lab.  The reason for completing the lab will ensure there is data avaibale for a demonstration at the end of the workshop.

The Launch API copmmand is discussed [here](https://docs.skillable.com/lod/lod-api/lod-api-launch.md).  It has a number of required parameters and will accept a lot of optional paramters.  We will only use a couple

- [] In Postman select the **GET Launch** option from the Lab On Demand Postman Collection
- [] Complete the Launch paramters as follows, if a parameter is listed below but not in the sample add it and if the parameter is listed in Postman but not below remove the tick, note you might need to scroll the Detials window up.

| Parameter Name | Value |
| ------ | ------|
| labId | +++116785+++ |
| userID | +++@lab.User.Email+++ |
| firstName | +++@lab.User.FirstName+++ |
| lastName | +++@lab.User.LastName+++ |
| +++variable-fnamevar+++ | *your first name* |
| +++variable-lnamevar+++ | *your last name* |

- [] In the details panel switch to the **Headers** tab.  This is where the API keyt will go
- [] In the first blank line enter:

| KEY | VALUE |
|-----|-------|
|+++api_key+++|+++@lab.Variable(api_key)+++|

- [] Press the Send button After a second or two a response should be returned.  The response will contain the Lab Instance ID as well as the Lab URL, that would be presented to a learner via the LMS.
  
>[!NOTE] In this next part you will use the browser on your local machine to ensure the graphics perform well.  Also complete the lab as the data will be valuable later in this workshop.  
  
 - [] Copy the URL and paste into your local browser.
 - [] Notice the lab has been personalised (firstname & lastname), with the data passed into the lab.
 - [] Complete the Lab and submit for scoring.
