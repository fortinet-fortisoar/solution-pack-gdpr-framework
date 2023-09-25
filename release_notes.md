# What's New

## Playbook Enhancements

- Updated the *Create Data Compliance Record* playbook to support data compliance record creation for both HIPAA and GDPR.

## Module Enhancements 

- Enhanced the **Data Compliance** module to be used by the both HIPAA and GDPR Framework solution packs.
    - For situations where both HIPAA and GDPR solution packs are deployed on the instance, the enhanced **Data Compliance** module avoids conflicts during the deployment of these solution packs.

### Data Compliance

- The Data Compliance module has new fields for it to work with HIPAA Framework solution pack. For the list of fields added, refer to [Data Compliance](./docs/contents.md#modules) section in Contents.

#### Key Store Module
- Added a Key Store Module to the SP
- Added GDPR KeyStore Records with 'Data Compliance' tag and with 'Key' value "GDPR". This records helps to determine which solution pack is deployed on the instance

## Content Enhancements

### Picklists
Picklists in the Data Compliance module have also been modified for them to work with HIPAA Framework solution pack. For the list of picklists now available, refer to [Picklists](./docs/contents.md#picklists) section in Contents.

<table>
    <tr>
        <td><strong>NOTE</strong></td>
        <td>Users of GDPR solution pack v1.0.0 must remove the fields and picklists mentioned in [Prerequisites](./docs/setup.md#prerequisites).</td>
    </tr>
</table>