### Lets launch a Lab into the Class

Having now created a class and setup monitoring you will now launch a lab into the class.

- [] Using the LDW-Launch command used earlier (it will be listed in the **@lab.Variable(Initials)-LDW Collection** or in a tab in Postman) make the following changes:
    - Change the labid to 116952
    - Add a new paramater for **classId** with a value of +++@lab.Lab.Instance.Id+++.  This is the same value we used to setup the class.
- [] The response from the Launch command will be similar to before and include the Url for the Lab Users access
- [] Switch to your local browser window showing the Lab Monitoring page you will see that Lab appear in a tile.  Over the next two minutes you will see the Lab boot up.
- [] Click on the tile and take control of the VM

### Summary
In lab 3 you have built a class, launched a lab within that class and taken control of the lab via instructor monitoring all by using API calls

- [] Let the instructor know you have finished Lab 3.

Press **next** to continue
