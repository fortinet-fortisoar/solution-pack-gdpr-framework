| [Home](https://github.com/fortinet-fortisoar/solution-pack-gdpr-framework/blob/release/1.0.1/README.md) | 
|--------------------------------------------| 
 
# Installation 
1. To install a solution pack, click **Content Hub** > **Discover**.    
2. From the list of solution pack that appears, search for and select **GDPR Framework**. 
3. Click the **GDPR Framework** solution pack card.    
4. Click the **Install** button on the bottom to begin installation. 

## Prerequisites

The **GDPR Framework** solution pack depends on the following solution packs.

| Solution Pack Name | Purpose                                                     |
|:-------------------|:------------------------------------------------------------|
| SOAR Framework v2.0.0    | 1. Required for Incident Response modules and Action playbooks 2. Required for "Was personal data affected?" field which acts as a trigger point for GDPR Framework Playbooks|

# Configuration 
For optimal performance of **GDPR Framework** solution pack, configure **Code Snippet** connector to extract and build address book of geo-specific DOP contacts.
- The connector comes pre-installed and hence needs only configurations. To configure **Code Snippet** connector, refer to [Configuring Code Snippet](https://docs.fortinet.com/document/fortisoar/0.0.0/fortisoar-built-in-connectors/1/fortisoar-built-in-connectors#CodeSnippet).