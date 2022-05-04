## Release Information

- Solution Pack Version: 1.0.0
- FortiSOAR™ Version Tested on: 7.2.0
- Authored By: Fortinet
- Certified: No

## Overview

### Introduction

**GDPR Framework Solution Pack** is designed to help users notify a personal data breach to the supervisory authority as per guidelines determined by General Data Protection Regulation(GDPR).

In the case of a personal data breach incident, as mandated in [GDPR Article. 33](https://gdpr-info.eu/art-33-gdpr/), the organization must notify the supervisory authority within 72 hours, and the notification must contain the following details:

- Nature of personal data breach
- Contact details of the data protection officer
- Consequences of the personal data breach
- Measures taken or proposed to remediate personal data breach
- Mitigating actions undertaken to minimize the risk

This solution pack provides a set of paybooks that enables users to gather all the necessary information and send it over to supervisory authority in time.

### Usage

For additional details, refer to [GDPR Framework Solution Pack documentation](https://github.com/fortinet-fortisoar/solution-pack-gdpr-framework/blob/develop/docs/solution-pack-guide.md)

## Prerequisites

|**Solution Pack**|**Purpose**|**Doc Link**|
| :- | :- | :- |
|SOAR Framework 1.0.0|Require for Incident Response modules|[Click here](https://github.com/fortinet-fortisoar/solution-pack-soar-framework/blob/develop/README.md)|

- Ensure that the **Code Snippet** connector is configured

## Contents

1. Report(s)

    - GDPR Assessment Report

2. Module(s)

    - Incidents
    - Contacts

3. Role(s)

    - Full App Permissions

4. Playbook Collection(s)

    - 10 - SP - GDPR Framework(10):

    |**Playbook Name**|**Description**|
    | :- | :- |
    |Create GDPR Assessment Tasks|Creates tasks for GDPR Assessment and links it to the incident|
    |Create GDPR Risk Assessment Incident|Creates and links the GDPR risk assessment incident and corresponding task to the parent incident|
    |Get Breach Report Reviewed and Approved by DPO|Sends personal data breach notification to Data Protection Officer (DPO) for review and approval of Data Breach Report.|
    |Get Data Protection Authorities Contact Details|Ingest contact details of Data Protection Authorities of various countries in the EU|
    |Get GDPR Risk Assessment Details|Collects GDPR assessment details complete the corresponding task|
    |Get Updated Data Breach Report from DPO|Get new/updated data breach report from DPO|
    |Notify Affected Individuals|Notifies affected users regarding the data breach|
    |Provide DPO and DPA Contact|Provide DPO and DPA contact details|
    |Send Data Breach Report to DPA|Send Data Breach Report to Data Protection Authority|
    |Set Breach Notification SLA|Sets Breach Notification SLA|

     **Warning:** It is recommended to clone these Playbooks before any customizations to avoid loss of information while upgrading the Solution Pack.
