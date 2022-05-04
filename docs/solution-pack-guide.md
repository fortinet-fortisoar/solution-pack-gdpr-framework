# Usage of GDPR Framework Solution Pack

## Solution Pack Workflow

- **Preliminary Personal Data Breach Details Gathering**
  - When a personal data breach is detected in an incident, choose the value of the **Was Personal Data Affected?** field as **Yes**.

    ![Personal Data Affected](media/personalDataAffected.png)

  - A pop-up appears that collects additional information related to the incident

    ![Personal Data Additional Details](media/personalDataAdditionalDetails.png)

  - The incident is updated with additional details and starts showing up during the remaining time to Notify Supervisory Authority
  - A New incident, dedicated to GDPR Assessment and the corresponding task, is created. The same is updated in the comments.

    ![Notification Timer](media/notificationTimer.png)

- **GDPR Assessment Incident**
  - Open the newly created GDPR incident; the corresponding tasks appear in the Description field and the task tabs. The tasks need to be complete within 72 Hours

    ![GDPR Tasks](media/gdprTasks.png)

## Tasks

- **Get GDPR Risk Assessment Information**
  - Open the `Get GDPR Risk Assessment Information` Task and click on **"GDPR Risk Assessment Form"** Button

    ![GDPR Risk Assessment Information Task](media/gdprRiskAssessmentInformationTask.png)

  - Fill up the Risk Assessment details in the pop-up

    ![Risk Assessment Details](media/riskAssessmentDetails.png)

  - Once the task is complete, it is highlighted in GREEN and the status is marked as **Complete**

    ![taskMarkedComplete](media/taskMarkedComplete.png)

- **Get DPO and DPA Contact**
  - Similarly, Collect DPO and DPA contact details under **Provide DPO and DPA Contact Details Task**

    ![DPO Contact Details](media/dpoContact.png)

  - Details provided reflect in the incident as shown, and the task is marked as complete

    ![Incident Details](media/incidentDetails.png)

- **Review and Approve Breach Report by DPO**
  - Open the `Review and Approve Breach Report by DPO` Task and click on the 'Notify Data Protection Officer' Button to get the information reviewed and approve the report to send to Data Protection Authorities

    ![Approve Data Breach Report](media/approveDataBreachReport.png)
  
Based on the inputs from DPO, the following new task is created

- **Communicate Affected Users of Breach**
  - If affected individuals are at **High** or **Medium** Risk, this new task is created to notify the individual of a data breach
  - Open the task and click on the `Notify Affected User` button
  - The notification should contain the following information
    - What happened? - Provide brief information on data breach
    - What Information Was Involved? - Provide information on what type of data was compromised
    - What Are We Doing? - Provide remediation/mitigation action are taken or planned to be taken
    - What You Can Do? - Provide advisory to the user about actions to be taken to minimize the risk

    ![notifyAffectedUsers](media/notifyAffectedUsers.png)

- **Get Updated Report from DPO**
  - If DPO rejects the data breach report, then this new task is created where the DPO can update the Data Breach Report and submit a new data
  - Open the task and click on the `Get Updated Breach Report` button

- **Notify Data Protection Authority**
  - This new task is created to Notify DPA of a data breach.
  - Open the task and click on the **Send Data Breach Report to DPA** Button
  - This task generates the following report and sends it to the DPA and resolves the GDPR Assessment Incident

  ![Data Breach Report](media/dataBreachReport.png)

  ![Incident Resolved](media/resolveIncident.png)
