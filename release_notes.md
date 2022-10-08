# What's New

- This solution pack is now **Certified**

## Module Enhancements 
- A new module **Data Compliance** now replaces the *Incident* module and all the fields previously used with `Incident` module are now part of *Data Compliance* module
  - A new Navigation menu was added for **Data Compliance**
  - **GDPR Assessment Report** has been updated to be compatible with the newly created **Data Compliance** module
- A new `GDPRReminderStatus` picklist keeps track of email reminders sent for SLA breach
- `RegulatoryBody` and `GDPRDataBreachType` are new picklists available

## Content Enhancements
- **Summary** tab contains more details and now has the following sections available as part of this solution pack's details:
    - A new category **Compliance and Reporting** &ndash; helps with filtering from the left pane when using the check-boxes under **Category**
    - A new tag **GDPR** &ndash; helps with filtering from the left pane when using the **Search By Tags** option
    - Added instructions to configure **Code Snippet** connector before execution of GDPR playbooks

## Playbook Enhancements
- Renamed following playbooks for enhanced understanding of functionality
    - **Create GDPR Risk Assessment Incident** renamed to **Create Data Compliance Record**
    - **Get Data Protection Authorities Contact Details** renamed to **Get DPA Contact Details**
- Added new playbooks to **10 - SP - GDPR Framework** playbook collection. For more details, 
    - **Check for SLA violation** 
    - **Send Reminder for SLA Breach**
    Refer to [Check for SLA violation Playbook](./docs/usage.md#check-for-sla-violation-playbook) section on how to configure these playbooks
    - A new schedule `GDPR - Check for SLA violation` added for **Check for SLA violation**
    - By default this schedule is `Inactive`, the user suppose to activate this schedule and set the desired frequency 
- GDPR playbook *Create Data Compliance Record*, now has two modes for execution
  - Test Mode
  - Production Mode
- Updated `Notify Affected Individuals` playbook, The task and the form associated with **Notify Affected Individuals** now also show the list of email IDs of the Affected Individuals

>**NOTE**: Users of GDPR solution pack v1.0.0 must remove the fields and picklists mentioned in [Prerequisites](docs/setup.md#prerequisites)
