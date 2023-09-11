# What's New

- This solution pack is now **Uncertified**

## Module Enhancements 

We have made changes in the module so it can be used by the both HIPAA and GDPR Framework solution packs. To support a situation when both HIPAA and GDPR solution packs are deployed on the instance, we are aligning the data compliance module in both of these solution packs to avoid any conflict during the deployment of these solution packs.
#### 1. Data Compliance Module
Newly Added Fields - Specifically for HIPAA Framework Solution pack

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
- Is A Breach Reportable
- Indicators
- Who Accessed PHI/ePHI Without Permission
- What Health Information Was Exposed
- Was The PHI/ePHI Encrypted
- Reminder Mail Status

#### 2. Key Store Module
- Added a Key Store Module to the SP
- Added GDPR KeyStore Records with 'Data Compliance' tag and with 'Key' value "GDPR". This records helps to determine which solution pack is deployed on the instance

#### 3. Asset Module

Rearranged the Asset List View Columns, the updated sequence of Asset fields in the list view
- Id
- Display Name
- Hostname
- MAC Address
- IP Address
- Device UUID
- Vendor
- Product
- Category
- Asset Criticality
- Asset State
- Asset Status
- Asset Risk
- Asset Registration Date
- Last Scanned On
- Property Of


## Content Enhancements
### Picklists
Added/Modified the below-mentioned picklists in the Data Compliance module
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

## Playbook Enhancements

- Updated `Create Data Compliance Record` playbook, The playbook is updated to support data compliance record creation for both HIPAA and GDPR.

>**NOTE**: Users of GDPR solution pack v1.0.0 must remove the fields and picklists mentioned in [Prerequisites](docs/setup.md#prerequisites)
