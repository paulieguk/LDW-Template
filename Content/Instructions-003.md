

## Lets try a command with no parameters.
You will use the Catalog command which is discussed here: [The Catalog command](https://docs.skillable.com/lod/lod-api/lod-api-catalog.md "The Catalog command")

When reviewing the command option notice the command accepts three input paramaters:

 - includeAll
 - LabSeriesID
 - OrganiationID

Notice all these paramaters are optional.  Also quickly review the Response (the outputs)  This command will return a list of:

 - Lab Series
 - Lab Profiles
 - Delivery Regions
 - Error code    



- [] In Postman exapnd the **Lab On Demand Postman Collection**
- [] Click **Catalog**.  Notice in the details panel that all parameters are selected and notice they are all listed on the **GET** command above
- [] Remove the tick from **includeAll** and as you do notice what happens in the **GET** statement
- [] Remove the tick from the other two options
- [] In the details panel switch to the **Headers** tab.  This is where the API keyt will go
- [] In the first blank line enter:

| KEY | VALUE |
|-----|-------|
|+++api_key+++|+++@lab.Variable(api_key)+++|

An optional description could be added if required.

- []Press the **Send** button
After a second or two a response should be returned listing what is available via the API Consumer in terms of Lab Series, Lab Profiles and Datacenters.

### Lets save this custom command in our own collection

- [] In Postman click the **New** button above the navigation panel
- [] Select **Collection**, you will see a new collection called **New Collection** is listed on the lower left
- [] At the top where **New Collection** is highlight change the name to +++@lab.Variable(initials)-LDW Collection+++, press **Enter**
- [] Switch back to the **Catalog** tab
- [] Click the down arrow next to Save and select **SaveAs** at the top right
- [] Set the Request name to +++LDW - Catalog+++
- [] Ensure you select **@lab.Variable(initials)-LDW Collection** in the Save to box, press **Save**

>[!ALERT] You have now saved your first custom API query with all the settings used including the API Key.  Be careful if you ever decide to export and share with others.

Press **next** to continue
