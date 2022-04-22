# Usage of GDPR Framework Solution Pack

## Solution Pack Workflow

- **Preliminary Personal Data Breach Details Gathering**
  - When a personal data breach is detected in an incident, then choose the value of the `Was Personal Data Affected?` field as 'Yes'

    ![Personal Data Affected](media/personalDataAffected.png)

  - A pop-up will appear that collects additional information related to the incident

    ![Personal Data Additional Details](media/personalDataAdditionalDetails.png)

  - The incident will be updated with additional and will start showing up during the remaining time to Notify Supervisory Authority
  - Also a New incident dedicated to GDPR Assessment and the corresponding task will be created. The same will be updated in the comments.

    ![Notification Timer](media/notificationTimer.png)

- **GDPR Assessment Incident**
  - Open the newly created GDPR incident, the corresponding tasks will be displayed in the Description field as well as in the task tabs. The tasks need to be completed within 72 Hours

    ![GDPR Tasks](media/gdprTasks.png)

## Tasks

- **Get GDPR Risk Assessment Information**
  - Open the `Get GDPR Risk Assessment Information` Task, Click on **"GDPR Risk Assessment Form"** Button

    ![GDPR Risk Assessment Information Task](media/gdprRiskAssessmentInformationTask.png)

  - Fill up the Risk Assessment details in the Pop-up

    ![Risk Assessment Details](media/riskAssessmentDetails.png)

  - Once the task is completed, it will mark GREEN and the status will be updated to 'Complete'

    ![taskMarkedComplete](media/taskMarkedComplete.png)

- **Get DPO and DPA Contact**
  - Similarly, Collect DPO and DPA contact details under 'Provide DPO and DPA Contact Details Task'

    ![DPO Contact Details](media/dpoContact.png)

  - All the provided details will be updated in the incident as shown below, and the task will be marked as completed

    ![Incident Details](media/incidentDetails.png)

- **Review and Approve Breach Report by DPO**
  - Open the `Review and Approve Breach Report by DPO` Task and click on the 'Notify Data Protection Officer' Button to get the information reviewed and approve the report to send to Data Protection Authorities

    ![Approve Data Breach Report](media/approveDataBreachReport.png)
  
Based on the inputs from DPO, the following new task will be created

- **Communicate Affected Users of Breach**
  - If affected individuals are at High or Medium Risk then this new task will be created to notify the individual of a data breach
  - Open the task and click on the `Notify Affected User` button
  - The notification should contain the following information
    - What happened? - Provide brief information on data breach
    - What Information Was Involved? - Provide information on what type of data was compromised
    - What Are We Doing? - Provide remediation/mitigation action are taken or planned to be taken
    - What You Can Do? - Provide advisory to the user about actions to be taken to minimize the risk

    ![notifyAffectedUsers](media/notifyAffectedUsers.png)

- **Get Updated Report from DPO**
  - If DPO rejects the data breach report then this new task will be created, where the DPO can update the Data Breach Report and submit a new data
  - Open the task and click on the `Get Updated Breach Report` button

- **Notify Data Protection Authority**
  - This new task gets created to Notify DPA of a data breach.
  - Open the task and click on the `Send Data Breach Report to DPA` Button
  - This task will generate the following report and send it to DPA and resolves the GDPR Assessment Incident

  ![Data Breach Report](media/dataBreachReport.png)

  ![Incident Resolved](media/resolveIncident.png)
