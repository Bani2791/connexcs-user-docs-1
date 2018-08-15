# Table of Contents

* [Table of Contents](#table-of-contents)
* [Carrier Management](#carrier-management)
    * [Adding New Carrier](#adding-carrier)
    * [Deleting Carriers](#deleting-carriers)
    * [Checking the Status](#checking-the-status)
    * [Searching Carrier](#searching-carrier)
    * [Customizing the View](#customizing-the-view)
    * [Edit Carrier](#edit-carrier)
         * [Stats](#stats)
         * [Reply-Management](#reply-management)
         * [Authentication](#authentication)
         * [Latest Calls](#latest-calls)
         * [Failover](#failover)
         * [Payment](#payment)  
         * [CDR](#cdr)  
         * [DID](#did)  
         * [Alerts](#alerts)  
    * [Code Consistency](#code-consistency)
    * [Consecutive Failures](#consecutive-failures)
    * [Special Considerations](#special-considerations)


# Carrier Management

Carriers can be easily and efficiently managed with the help of **Connex.** **Connex** allows you to not only add, edit and delete carriers but also lets you view the columns you want to see. 

To go to the **Carrier**,you can expand the **_Management_** tab from the left pane and select **"Carrier".**


![alt text][carrier-list]

## Adding Carrier

![alt text][add-carriers]

You can add new **Carriers** by following the simple procedure.

1. Click the **'+'** button.
2. Enter the details of the **carrier.**
3. Click the **Save** button when all the details are entered properly.

Figure: The dialog box for adding the **Carrier.**

![alt text][carrier-details]
        
The brief description of fields present in the above form, is given below:
        
**Carrier Name:** Here add the name of your Carrier.

**Channels:** Please add the number of channels (Ports) required in digits only. Setting this to ZERO will allow unlimited channels.

**CPS:** You can add the number of "Calls Per Second" but in digits only.

**PayPal Email:** Please add the "PayPal Email" of your **Carrier.**

**Website:** Here add the Website address of your Carrier.

**Portal URL:** Add the Portal URL for your carrier in this field. eg:portal.yourcarrier.com 

**Portal Username:** Please enter the Portal Username. This could be either your email address or user name.

**Portal Password:** Enter the password you use for logging into your carrier portal.

**Portal Access:** Here you need to choose either Yes or No from the drop down menu to allow your carrier to access the portal.

**Status:** You can set/select the "Status" of the your **Carrier.** here. The Status dropdown menu options are:

1. Active - your carrier is available to process the calls.
2. Inactive - your carrier is disabled.
3. Pending Approval - means that you are waiting for acceptance from your carrier at which point they can then be set to either of the      two options.

**Currency:** Here you need to choose your preferred "Currency" from the dropdown menu options.

**Address:** You need to add the "Address" of your **Carrier** including country and postcode/ZIP code.

**First Reply Timeout:** This is the length of time that you give for the carrier to respond after the **first invite**. Default value     is set to 30 seconds.

**PDD Timeout:** This is the length of time that you give for the carrier to respond to the call. The default value is 5 seconds.

**Ring Timeout:** This is the length of time that the call is allowed to ring before it times out and sends a cancel message. The         default value is 60 seconds.

## Deleting Carriers

You can also delete the existing **Carriers** from the list if you want to. 

1. Select the **Carrier** from the list by check marking the entire row.

2. Click on the **Delete** button, i.e. trash icon.

## Checking The Status

![alt text][carriers-sorting]

If you need to check/alter the status of the **Carriers.** 

1. Click on the button named **Active.**
2. Select an option from the dropdown menu.
3. Results will show up according to the selected option.

## Searching Carrier

If you have to search for any information about a **Carrier** you can write a query in the **Search** text field.

## Customising The View

You can customize the view of your **Carriers** page and select only the columns which you want to view.
On the extreme right, click on the menu button, and check the columns you want to view.

## Edit Carrier

In order to edit a **Carrier**, select a **Carrier** from the list. A new page will open. Follow the procedure given below:

1. Press the **"Edit Carrier"** button.
2. Edit the details and press **"Save"** button.
See below:

![alt text][carrier-dashboard]

### Stats

You can view various stats by clicking on the tab “Stats”.
![alt text][carrier-stats] 

### Reply Management

There is a special module in Connex for replying efficiently and that is Reply Management.
There are codes on the basis of which action and responses are set. You can customize your responses too.
 
Choose the “Replace” radio button and then “New Code” and “New Reason” field would appear. Here, choose a code and fill the reason of your choice.

![alt text][carrier-reply] 
 
### Authentication

You can add your Carrier IP address in this

![alt text][carrier-authentication] 
 
You can also add new IP for authentication, by clicking on the “+” sign on the extreme right. 

![alt text][carrier-ip-1] 
 
Add the details into the Basic and Advanced tabs to complete the addition of authenticated IP. Then click 'Save'.

### Latest Calls

“Latest Calls” is the tab next to Authentication. Here you can find all the calls you have made, lately.
 
You can simulate a call too by clicking the green button, labelled “Simulate”.

![alt text][carrier-calls] 

### Failover
 
 “Failover” are the calls which were not made successfully. A list of failover calls is shown in this tab.
 
![alt text][carrier-failover] 
 
### Payment

“Payment” tab lets you see all the payments made so far. You can add a new payment by clicking on the “+” sign.
 
Fill in the payment information and click “Save”.

![alt text][carrier-payment] 
 

#### CDR

“CDR” tab lets you check all your CDRs. You can also recalculate a CDR for a specific month by entering the dates and clicking on “Recalc CDR”.

![alt text][carrier-cdr] 
 
### DID

“DID” tab lets you check your list of DIDs.  You can add a new DID by clicking on the “+” on the extreme left.
 
After adding the details, remember to click “Save”.

![alt text][carrier-did]

### Alerts

The last tab is the "Alerts" tab. It allows you to generate alerts to your customers when some specific events are triggered. You can view all your alerts by clicking on this tab.

You can also add a customised alert by clicking on the "+" sign.

![alt text][carrier-alert-1]

You need to give the alert a name such as: Low Balance Alert,

Next select the email address or phone number to whom you wish the alert to go to,

The Area is the place that is being monitored ie Balance,

The Operator is the comparitor to which the threshold is compared. If the Operator is set to eg >$50 and the Threshold is set to $50 then the Alert will be triggered and sent out to the recipient.

Click "Save" and a new alert will be created.

![alt text][carrier-alert-2]

## Code Consistency

This measures the changes of response codes on the SAME number that have been returned from the carrier. It is useful for identifying if the carrier is using routes of different quality or generally poor quality overall. Good carriers will have a 100% code consistency.

The metric only takes into account 200 and 404's.

## Consecutive failures
The consecutive failures system is a primitive way of measuring the ability of a carrier to connect calls, once a call connects the counter is reset and once a call fails the counter is incremented by one.
This can lead to a false positive if the customer is sending a lot of missed call traffic or calling bad numbers, however in general the counter is one of the quickest ways to establish when a route is failing.

## Special Considerations
_Bandwidth.com_ have diverged from the SIP spec and expose an internal IP address which is required to be presented in sequential requests. To ensure compatibility set the switch manafacturer to ```bandwidth.com```



[carrier-list]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/99.png "Carrier-List"
[add-carriers]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/100.png "Add-Carrier"
[carrier-details]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/101.png "Carrier-Details"
[carriers-sorting]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/102.png "Carriers-Sorting"
[carrier-dashboard]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/103.png "Carrier-Dashboard"
[carrier-stats]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/104.png "Carrier Stats"
[carrier-reply]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/105.png "Carrier Reply"
[carrier-authentication]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/106.png "Carrier Authentication"
[carrier-ip-1]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/107.jpg "Carrier IP 1"
[carrier-calls]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/108.png "Carrier Calls"
[carrier-failover]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/109.png "Carrier Failover"
[carrier-payment]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/110.png "Carrier Payment"
[carrier-cdr]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/111.png "Carrier CDR"
[carrier-did]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/112.png "Carrier DID"
[carrier-alert-1]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/113.png "Carrier Alert-1"
[carrier-alert-2]: https://raw.githubusercontent.com/digipigeon/connexcs-user-docs/master/new-images/114.png "Carrier Alert-2"