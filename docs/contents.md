| [Home](../README.md) | 
|----------------------| 
 
# Contents

## Reports

- GDPR Assessment Report

## Modules

- Data Compliances. Following new fields help this module to work with HIPAA Framework solution pack:

    - Are The Affected Individuals' Contact Details Outdated
    - Has HSO Reviewed The PHI Breach Report
    - Is Law Enforcement Agency Notified
    - Individual Notice Approved
    - Steps Taken To Investigate The Breach
    - Root Cause Analysis Findings
    - Technical Fix Summary
    - Actions for Applying Technical Fix
    - CE Phone
    - CE Email
    - CE Street Address
    - CE Name
    - HSO Email
    - HSO Phone
    - HSO Name
    - Describe Other Location Of Breach
    - Location Of Breach
    - Clinical PHI Exposed In Breach
    - Describe Other Actions Taken
    - Actions Taken In Response To Breach
    - Is Media Notice Required
    - Is Substitute Notice Required
    - Safeguards In Place Before Breach
    - Financial PHI Exposed In Breach
    - Demographic PHI Exposed In Breach
    - Type Of PHI Involved In Breach Other
    - Brief Description Of The Breach
    - Type Of PHI Involved In Breach
    - Breach Unpaused Date
    - Is PHI Misuse Or Disclosure Foreseeable
    - Was The PHI/ePHI Accessed Impermissibly
    - Indicators
    - Who Accessed PHI/ePHI Without Permission
    - Was The PHI/ePHI Encrypted

- Contacts

## Picklists
- Following picklists in the Data Compliance module have also been modified, and some added, for them to work with HIPAA Framework solution pack:

    - ClinicalPHIType 
    - Contact Title
    - DemographicPHIType
    - FinancialPHIType
    - GDPRDataBreachType
    - GDPREUCountryList
    - GDPRReminderStatus
    - PHIBreachLocation
    - PHIBreachResponseActions
    - PHISafeguardType
    - ProtectedHealthInformationType
    - RegulatoryBody

## Roles

- Full App Permissions

## Playbook Collection

| 10 - SP - GDPR Framework|
|:------------------------|

| Playbook Name                                  | Description                                                                                                             |
|:-----------------------------------------------|:------------------------------------------------------------------------------------------------------------------------|
| Check for SLA violation                        | Checks for breach notification violation and update SLA status to Missed                                                |
| Reminder for SLA Breach                        | Sends reminder for the notification SLA Breach                                                                          |
| Set Breach Notification SLA                    | Sets Breach Notification SLA                                                                                            |
| Create GDPR Assessment Tasks                   | Creates tasks for GDPR Assessment and links them to the incident                                                        |
| Create Data Compliance Record                  | Creates and links a data compliance record and corresponding task to the parent incident                                |
| Get Breach Report Reviewed and Approved by DPO | Sends personal data breach notification to Data Protection Officer (DPO) for review and approval of Data Breach Report. |
| Get DPA Contact Details                        | Ingest contact details of Data Protection Authorities of various countries in the EU                                    |
| Get GDPR Risk Assessment Details               | Collects GDPR assessment details and complete the corresponding task                                                    |
| Get Updated Data Breach Report from DPO        | Get new/updated data breach report from DPO                                                                             |
| Notify Affected Individuals                    | Notifies affected users regarding the data breach                                                                       |
| Provide DPO and DPA Contact                    | Provide DPO and DPA contact details                                                                                     |
| Send Data Breach Report to DPA                 | Send Data Breach Report to Data Protection Authority                                                                    |

<table>
    <tr>
        <td><strong>WARNING</strong></td>
        <td>It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.</td>
    </tr>
</table>

| [Installation](./setup.md#installation) | [Configuration](./setup.md#configuration) | [Usage](./usage.md) |
|-----------------------------------------|-------------------------------------------|---------------------|
