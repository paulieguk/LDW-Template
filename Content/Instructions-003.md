# 003 - Your first API command

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
- [] In the details panel switch to he **Headers** tab.  This is where the API keyt will go.
- [] In the first blank line enter:

| KEY | VALUE |
|-----|-------|
|+++api_key+++|+++@lab.Variable(api_key)+++|

An optional description could be added if required.

- []Press the **Send** button
After a second or two a response should be returned listing what is available via the API Consumer in terms of Lab Series, Lab Profiles and Datacenters.


