##Scenario

In Lab 3 you will build a class and run labs within that class.  This will allow you to see the Lab Monitoring feature, often shown within the Skillable TMS, accessed via API.  This feature requires two steps for setup.

1. Create a Class
1. Retrive the Instructor Lab Monitor URL
1. Launch a lab within the Class

### Lets build a Class

Review the parameters for the [**GetOrCreateClass API**](https://docs.skillable.com/lod/lod-api/lod-api-get-or-create-class.md) call as you complete the Postman request.  The GetOrCreateClass API call will returned an existing class if one matches the input paramaters or if no class exists LOD will create a new one.

 - [] In Postman select the GET GetOrCreateClass API command
 - [] Set the parameters for the class using the values below:

| Parameter Name | Value |
| ------ | ------|
| id | +++@lab.LabInstanceID+++ |
| name | +++@lab.User.FirstName-Class+++ |
| start |  |
| end | +++1648771200+++ |
| expires | +++1648771200+++ |

>[!Help] <summary> Epoch time information </summary>
><details>
 Epoch time value 1648771200 = 1st April 2022 00:00:00hrs GMT you can confirm this on [https://www.epochconverter.com/](https://www.epochconverter.com/)
 </details>

- [] Enter the API Key details

| KEY | VALUE |
|-----|-------|
|+++api_key+++|+++@lab.Variable(api_key)+++|

- [] Press the Send button After a second or two a response should be returned.  The response will contain details about the class.  Notice the Url field in the response is set to NULL.  Ths shows our API consumer is setup as a new customer not an existing one.  We now need to setup monitoring and also launchs labs within the class.
- [] Save this API command as +++LDW - GetOrCreateClass+++ in the **@lab.Variable(initials)-LDW Collection**

Press **next** to continue
