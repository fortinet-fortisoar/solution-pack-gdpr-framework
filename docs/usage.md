| [Home](../README.md) |
|----------------------|

# Usage

## Playbook Execution Modes

You can execute the GDPR playbooks in *Test Mode* as well as in *Production Mode*

- The playbooks are by default configured to execute in *Test Mode*
  - The *Test Mode* uses a test email address for all email communication towards Data Protection Officer (DPO), affected individuals, or Data Protection Authority(DPA)
  - The *Production Mode* uses actual email addresses  of relevant authorities and stakeholders

>**WARNING**: Please be careful of the email addresses you use, as data breach notification emails are sent to these addresses. Hence, while in *Test* mode, do not use actual DPO and DPA email addresses.

### Test Mode

To change the execution mode to *Test* make the following changes:

1. Go to the *Create Data Compliance Record* playbook under the **10 - SP - GDPR Framework** collection and open the *Configuration* step

    ![Execution Mode Configuration](./res/execution-mode-configuration.png)

2. Modify the value of the `testMode` variable to `true`.
3. Change the value of the `testEmail` variable to a valid email address capable of receiving all GDPR email notifications.
  >**WARNING**: When in *Test* mode, the value of the `testEmail` variable must not be empty.

    ![Execution Mode Configuration Parameters](./res/execution-mode-configuration-parametes.png)

### Production Mode

To change the execution mode to *Production* make the following changes:

1. Go to the *Create Data Compliance Record* playbook under the **10 - SP - GDPR Framework** collection and open the *Configuration* step

    ![Execution Mode Configuration](./res/execution-mode-configuration.png)

2. Modify the value of the `testMode` variable to `false`.
3. Keep the `testEmail` variable blank.

    ![Execution Mode Configuration Parameters](./res/execution-mode-configuration-parameters.png)

>**NOTE**: As a failsafe, `_demo` is appended to DPA's email as shown in the following image. This action prevents any accidental sending of mail to the Data Protection Authority (DPA).

![DPA Email Append](./res/dpa-appended-email.png)

In *Production* mode before you execute **Provide DPO and DPA Contact** playbooks, make the following changes:
1. Go to **Provide DPO and DPA Contact** playbook.
2. Open the *Get DPA Contact* step and remove `_demo` from `dpaEmail` variable as shown.
    ![Provide DPO and DPA Contact Changes](./res/provide-dpo-and-dpa-contact.png)

## Check for SLA Violation Playbook

This playbook sends progressive SLA breach reminder emails. To set threshold values for reminder notifications, make the following configuration changes:

1. Goto **Check for SLA violation** Playbook and open the *Configuration* step.
2. The reminder threshold value is in hours. Change values of the following variables
    - `firstReminderSLA`: The default value is 24 Hours which means the first reminder is sent when the SLA time remaining is less than 24 hours left.
    - `secondReminderSLA`: The default value is 4 Hours which means the second reminder is sent when the SLA time remaining is less than 4 hours left.
        ![Reminder Email Configuration Setting](./res/reminder-mail-configuration.png)

A third and final reminder, of SLA breach, is sent after the completion of 72 hours.

## Gathering Details on Personal Data Breach

1. When a personal data breach is detected in an incident, choose the value of the **Was Personal Data Affected?** field as **Yes**.

    ![Personal Data Affected](./res/personal-data-affected.png)

2. A pop-up appears that collects additional information related to the incident

    >**NOTE:** When playbooks are executed in *Test* mode, the **Green** icon shown in the following screenshot appears in all the tasks related to this solution pack
    >
    >![Personal Data Additional Details](./res/personal-data-additional-details.png)
    >
    >Similarly, when playbooks are executed in *Production* mode, a **Red** icon shown in the following screenshot appears
    >
    >![Personal Data Additional Details PROD](./res/personal-data-additional-details-prod.png)

3. Select **GDPR** in **Regulatory Body** and provide the required information

    ![Personal Data Details](./res/personal-data-details.png)

4. A New Data Compliance Record, dedicated to GDPR Assessment and the corresponding task, is created. The same is updated in the Incident comments.

    ![Incident Comments](./res/incident-comments.png)

### GDPR Assessment Data Compliance Record

- Open the newly created GDPR Data Compliance Record; the corresponding tasks appear in the Description field and the task tabs. The tasks need to be completed within 72 Hours.

- The Data Compliance Record is also updated with additional details and starts showing up the remaining time to notify the supervisory authority.

    ![Notification Timer](./res/notification-timer.png)

## Submit Risk Assessment Information

1. Open the **Submit Risk Assessment Information** Task and click the **Submit Risk Assessment Information** button.

    ![GDPR Risk Assessment Information Task](./res/gdpr-risk-assessment-information-task.png)

2. Enter the Risk Assessment details in the pop-up that appears.

    ![Risk Assessment Details](./res/risk-assessment-details.png)

3. Once the task is complete, it is highlighted in **green** and the status is marked as **Complete**.

    ![taskMarkedComplete](./res/task-marked-complete.png)

## Provide DPO and DPA Contact Details

1. Open the **Submit Risk Assessment Information** Task and click the **Submit Risk Assessment Information** button.

2. Similarly, Collect DPO and DPA contact details under **Provide DPO and DPA Contact Details** Task

    ![DPO Contact Details](./res/dpo-contact.png)

3. Details provided reflect in the created data compliance record as shown, and the task is marked as complete

    ![Incident Details](./res/incident-details.png)

## Notify Data Protection Officer

1. Open the **Notify Data Protection Officer** task and click the **Notify Data Protection Officer** button. This sends an email to the DPO.

2. The DPO clicks the link in the email to review and approve the information shown in the following screen.

    ![Approve Data Breach Report](./res/approve-data-breach-report.png)
  
3. Details provided by DPO is reflected in the created data compliance record as shown, and the task is marked as complete

    ![Approve Data Breach Report](./res/dpo-assessment-details.png)

Based on the inputs from DPO, new tasks may be created. Following flow diagram explains when a new task is created:

![New task creation flow](./res/task-creation-flow.svg)

## Get Updated Report from DPO
If DPO rejects the data breach report, then this new task is created where the DPO can update the Data Breach Report and submit new data.
1. Open the task and click the **Get Updated Breach Report** button.
2. The process now is the same as described in [Notify Data Protection Officer](#notify-data-protection-officer) section.

## Notify Affected Users

1. Open the task and click the **Notify Affected Individuals** button
2. The notification should contain the following information
    - What happened? - Provide brief information on data breach
    - What Information Was Involved? - Provide information on what type of data was compromised
    - What Are We Doing? - Provide remediation/mitigation action are taken or planned to be taken
    - What You Can Do? - Provide advisory to the user about actions to be taken to minimize the risk

        ![notifyAffectedUsers](./res/notify-affected-users.png)

## Notify Data Protection Authority (DPA)
This new task is created to Notify DPA of a data breach.
1. Open the task and click the **Send Data Breach Report to DPA** Button.
2. This task performs the following actions:
    - Generates the following report and sends it to the DPA
    - Resolves the GDPR Compliance record
    - Completes the task **Perform GDPR Assessment** associated with the parent incident

    ![Data Breach Report](./res/data-breach-report.png)

    ![Compliance Record Resolved](./res/resolve-incident.png) 

    ![Incident Task Completed](./res/incident-task-completed.png)