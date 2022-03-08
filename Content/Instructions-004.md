# 004 - Lets launch a Lab

### In this activity you will launch a lab and then complete the lab.  The reason for completing the lab will ensure there is data avaibale for a demonstration at the end of the workshop.

The Launch API copmmand is discussed [here](https://docs.skillable.com/lod/lod-api/lod-api-launch.md).  It has a number of required parameters and will accept a lot of optional paramters.  We will only use a couple

- [] In Postman select the **GET Launch** option from the Lab On Demand Postman Collection
- [] Complete the Launch Paramters as follows, if a parameter is listed below but not in the sample add it and if the parameter is listed in Postman but not below remove the tick:

| Parameter Name | Value |
| ------ | ------|
| labId | +++116785+++ |
| userID | +++@lab.User.Email+++ |
| firstName | +++@lab.User.FirstName+++ |
| lastName | +++@lab.User.LastName+++ |
| fnamevar | <your first name> |
| lnamevar | <your last name> |

- [] In the details panel switch to the **Headers** tab.  This is where the API keyt will go
- [] In the first blank line enter:

| KEY | VALUE |
|-----|-------|
|+++api_key+++|+++@lab.Variable(api_key)+++|




