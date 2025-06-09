# MS Dynamics Quality Assurance Test Scripts

[Script 1](QA.md#script-1)

[Scipt 2](QA.md#script-2)

##  Script 1

**Part 1**

As a team lead with _Append_ permissions in the Sandbox environment
 
1. From a _Team_ page from the _Email notifications_ tab, enable the **Stale On Hold Case Notifications** setting

 
**Part 2**

As a CSR on the Testing Team in the Sandbox environment where the following is true:

 * The "Stale On Hold Case Notifications" have been enabled (see above)
 * There is at least one case with a status of _On Hold_

 Note: In the Sandbox environment, the automation will be run in a demo state that should send emails out for any _On Hold_ cases not modified in 1 minute. In Production, this query will be every 30 days.
___

1. Notify the Developer that you wish to begin testing this ticket
2. Create a case
3. Change the status of the case to _On Hold_

**Result**

You should receive an email within a few minutes that states, "You have Cases that have been On Hold for 30 days or more."


---

##  Script 2

As a CSR on the Testing Team in the Sandbox environment

1. From _My Active Cases_ screen, click the **New Case** button
2. Create a case, save, and submit
3. From the _Update Status_ menu, select **Mark Duplicate**
![Mark Duplicate](https://github.com/user-attachments/assets/0fd30524-e915-4810-afc5-e09cbcf98cff)
 
 The _New Case Update_ side panel opens.
 
 4. From the _New Case Update_ side panel, click the field. A list of cases diplay.
 5. If you try to mark the current case as its own duplicate, you will receive an error.
 ![Error Message](https://github.com/user-attachments/assets/37ca88f5-fbfc-4700-986a-0e04d9c25ecb)

 7. Select a different case and click the **Save** button

**Result**

 The case becomes _Read-only: Resolved_ and status _Duplicate_
![Case Read-only: Resolved](https://github.com/user-attachments/assets/5edbde52-7db1-42cc-841d-8d7b29d77fca)



---

[Return to main page](https://jenpetsmit.github.io/)

&nbsp;
