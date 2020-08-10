# Routing Global
**Routing Global** allows you to create routing templates that can be applied to multiple customers. This is ideal when all or multiple customers are using a repeatable configuration, either the same type of route or the same routing settings. When you need to apply a change to routing for multiple customers, you only need to update the template. 

## Setup
To setup **Routing Global** template, first create it then apply it to the customer account(s) using the **Tag** field. 

**Create the template**

1. Go to Management > Routing Global
2. Click the **`+`** to create a new template
3. Complete the fields (see [Advanced Routing configuration](https://staging--connexcs-docs.netlify.app/customer/routing/#advanced-routing-configuration) for details)

    ![alt text][routing-global]

4. The **Tag** field is essentially the name of the template
5. Select **`Save`**.

**Assign the template**

For each customer that needs the new template:

1. Navigate to Management > Customer and select the customer
2. Select **`Edit`** in the upper right corner
3. On the config tab, select the new template under **Tags**
4. Save the customer configuration. 


!!! info "Using Routing Global and Script Forge"
    Routing Global templates can't be used to set routing details with ScriptForge (Vars box). With appropriate design, these can be configured directly under Customer Routing.

[routing-global]: /misc/img/routing-global1.png "Edit Global Routing"