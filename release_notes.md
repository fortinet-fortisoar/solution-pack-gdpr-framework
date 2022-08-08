# What's New

- This solution pack is now **Certified**
- **Summary** tab contains more details and now has following sections available as part of this solution pack's details:
    - A new category **Compliance and Reporting** &ndash; helps with filtering from the left pane when using the check-boxes under **Category**
    - A new tag **GDPR** &ndash; helps with filtering from the left pane when using the **Search By Tags** option
    - Added instructions to configure "Code Snippet" connector before execution of GDPR playbooks
- A new module **Data Compliance** has been intoduced
- A new Navigation menu added for 'Data Compliance'
- Added new playbooks to **Check for SLA violation** and to **Send Reminder for SLA Breach**
- Updated **GDPR Assessment Report** to be compitable with newly created module i.e 'Data Compliance'
- Added a provision to execute GDPR playbooks either in **Test Mode** or in **Production Mode**
- The task and te form associated with **Notify Affected Individuals** now also shows list of email-IDs of the Affected Individuals

**Note:**
* It is recommended to the users who have already installed the GDPR SP v 1.0.0 to remove the below fields and picklists from the Incident Module
    * Fields
        - Breach Detection Date 
        - Breach Occurrence Date 
        - Breach Notify Due Date 
        - Breach Paused Date 
        - Breach Notification SLA(Picklist - SLAState)
        - Was the data encrypted? (Picklist - YesNo Picklist)
        - Was the exposure resolved? (Picklist - YesNo Picklist)
        - Is harm, risk or misuse foreseeable? (Picklist - YesNo Picklist)
        - What was the data format? 
        - What was the data source? 
        - Company Name 
        - Company Size 
        - Company City
        - Company Country 
        - Cause of Data Breach 
        - Type of Data Breach (Picklist - DataBreachType)
        - Data Type 
        - Where data was hosted?
        - Repercussions of Breach
        - Mitigation Actions
        - No. of Affected Users 
        - No. of Affected Data Records 
        - Affected Users Emails
        - Any Additional Information
        - Data Regulator (Picklist - GDPREUCountryList)
        - DPA Website
        - DPA Email
        - DPA Address
        - DPO Telephone
        - DPO Email
        - DPO Name
        - Summary of DPO Advice
        - Is Valid Breach? (Picklist - YesNo Picklist)
        - Is DPIA Required?
        - Reason To Perform DPIA
        - Impact Severity on Affected Users (Picklist - Severity)
        - Measures to Reduce Future Risks

    * Picklists
        - DataBreachType
        - YesNo Picklist