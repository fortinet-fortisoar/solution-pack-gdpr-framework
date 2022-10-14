| [Home](../README.md) | 
|----------------------| 
 
# Installation 
1. To install a solution pack, click **Content Hub** > **Discover**.
2. From the list of solution packs that appear, search for and select **GDPR Framework**.
3. Click the **GDPR Framework** solution pack card.
4. Click the **Install** button on the bottom to begin the installation.

## Prerequisites

The **GDPR Framework** solution pack depends on the following solution packs.

| Solution Pack Name    | Purpose                                                                                                                                                                                           |
|:----------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| SOAR Framework v2.0.0 | <ol><li>Required for Incident Response modules and Action playbooks</li><li>Required for "Was personal data affected?" field which acts as a trigger point for GDPR Framework Playbooks</li></ol> |

If you have already installed the GDPR solution pack v1.0.0, remove the following fields and picklists from the **Incident** Module

### Fields
- Breach Detection Date 
- Breach Occurrence Date 
- Breach Notify Due Date 
- Breach Paused Date 
- Breach Notification SLA(Picklist - SLAState)
- Was the data encrypted? (Picklist - YesNo Picklist)
- Was the exposure resolved? (Picklist - YesNo Picklist)
- Is harm, risk, or misuse foreseeable? (Picklist - YesNo Picklist)
- What was the data format? 
- What was the data source? 
- Company Name 
- Company Size 
- Company City
- Company Country 
- Cause of Data Breach 
- Type of Data Breach (Picklist - `DataBreachType`)
- Data Type 
- Where data was hosted?
- Repercussions of Breach
- Mitigation Actions
- No. of Affected Users 
- No. of Affected Data Records 
- Affected Users' Emails
- Any Additional Information
- Data Regulator (Picklist - `GDPREUCountryList`)
- DPA Website
- DPA Email
- DPA Address
- DPO Telephone
- DPO Email
- DPO Name
- Summary of DPO Advice
- Is Valid Breach? (Picklist - `YesNo`)
- Is DPIA Required?
- Reason To Perform DPIA
- Impact Severity on Affected Users (Picklist - `Severity`)
- Measures to Reduce Future Risks

### Picklists
- `DataBreachType`
- `YesNo`

# Configuration 
For optimal performance of **GDPR Framework** solution pack, configure **Code Snippet** connector to extract and build an address book of geo-specific Data Protection Authority (DPA) contacts.
> The connector comes pre-installed and hence needs only configurations. To configure **Code Snippet** connector, refer to [Configuring Code Snippet](https://docs.fortinet.com/document/fortisoar/0.0.0/fortisoar-built-in-connectors/1/fortisoar-built-in-connectors#CodeSnippet).