# Quality Assurance Test Scripts

[Script 1](QA.md#script-1)

[Scipt 2](QA.md#script-2)

Here is my first QA test script I wrote. 

##  Script 1

### Goal 1 For Team Lead

**Set Up**

A team lead with the following:
 * Append permissions
 
1. From a Team page from the Email notifications tab, enable the "Stale On Hold Case Notifications" setting

 
### Goal 2 For CSR

**Set Up**

A CSR on the Testing Team where the following is true:

 * The "Stale On Hold Case Notifications" have been enabled (see above)
 * There is at least one case with a status of _On Hold_

1. Notify the Developer that you wish to begin testing this ticket.
   * In the Sandbox environment, the automation will be run in a demo state that should send emails out for any _On Hold_ cases not modified in 1 minute.
   * In Production, this query will be every 30 days.
2. Create a case and change the status of the case to _On Hold_

**Result**

You should receive an email within a few minutes that states, "You have Cases that have been On Hold for 30 days or more."

&nbsp;

##  Script 2

### Goal - Mark duplicate cases as duplicate

1. From _My Active Cases_ screen, click the **New Case** button.
2. Create a case, save, and submit
3. From the _Update Status_ menu, select **Mark Duplicate**
![Mark Duplicate](https://github.com/user-attachments/assets/0fd30524-e915-4810-afc5-e09cbcf98cff)
 
 The _New Case Update_ side panel opens.
 
 4. From the _New Case Update_ side panel, click the field. A list of cases diplay.
 5. If you try to mark the current case as its own duplicate, you will receive an error.
 ![Error Message](https://github.com/user-attachments/assets/37ca88f5-fbfc-4700-986a-0e04d9c25ecb)

 7. Select a different case and click the **Save** button

 The case becomes Read-only: Resolved and status Duplicate


---

[Return to main page](https://jenpetsmit.github.io/)

&nbsp;
