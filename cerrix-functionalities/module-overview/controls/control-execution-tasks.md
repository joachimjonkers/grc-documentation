# Control Execution Tasks

{% hint style="info" %}
**Video Tutorial**

Prefer to watch instead of read? Have a look at our [#control-execution-tasks](../../../best-practices-and-guides/video-tutorials.md#control-execution-tasks "mention") Video Tutorial
{% endhint %}

Control execution tasks are essential for ensuring that your risk and compliance controls are regularly tested and updated. In CERRIX, these tasks are linked directly to your controls, providing transparency and traceability throughout your compliance program.

This guide will cover:

* The process of activating control execution for a control.
* How to create and manage control execution tasks.
* Key interfaces for responsible and reviewer roles.

## Activating Control Execution for a Control

To start using control execution tasks, you must first activate control execution for the relevant control:

1. Go to the Controls module.
2. Select the control you want to enable execution for.
3. Locate the Control Execution section within the control’s detail page.
4. Enable the Control Execution toggle.
5. Save the changes.
6. Wait for the screen to refresh automatically. After saving, 'Control execution' will appear in the upper right corner of the screen.

<figure><img src="../../../.gitbook/assets/image (4).png" alt="" width="563"><figcaption></figcaption></figure>

## Creating Control Execution Tasks

### Option 1: Creating a Task Series (Recurring Tasks)

To create recurring control execution tasks, you need to create a new task series:

1. Click on the 'Control execution' button. A new tab will open.
2. Stay on the 'Recent and upcoming' tab. Initially, no control execution tasks will be shown.
3. Open the 'Task series' tab and click on 'add'. A new tab will open showing the details page of the task series.
4. Define the task series by filling in the following details:
   * **Name:** Enter a name for the task series.
   * **Responsible(s):** Select one or more individuals responsible for the tasks.
   * **Notifications:** Select when automatic notifications must be sent to the responsible(s).
   * **Description:** Provide a clear description for the execution steps of the task. This is crucial for quality execution and evidence.
   * **Task Type:** Currently, only 'control execution' is available.
   * **Reviewer(s):** Optionally, select one or more reviewers. If a reviewer is selected, a workflow will be created for all tasks in this series.
   * **Task Score Options:** Choose whether the responsible must give a score, has the option to give a score, or if the score field should be invisible. Select 'not required' as a task score.
5. Navigate to the end of the page to plan the control task series.
6. Select the frequency for the recurring task:
   * **Yearly:** For example, repeat 1, first Monday.
   * **Monthly:** For example, repeat 3, first Monday (each quarter).
   * **Weekly:** For example, repeat 1, select Monday.
   * **Daily**.
7. Fill in the **Start date** (e.g., 1 January 2025) and **End date** (e.g., 31 December 2025) for the task series.
8. Click 'Save' to create the task series.
9. After the page refreshes, the task series will be created based on the selected frequency. Only the end date can now be changed.
10. Close the task series tab and refresh the control execution screen to get an overview of the created task series. The task series that was just created will be shown.
11. Open 'Recent and upcoming' to view the individual tasks.

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

### Option 2: Creating an On-Event Control Execution Task

To create an on-event control execution task:

1. Open 'All control executions'.
2. Click 'add'.
3. Fill in the required fields. This 'on event' control execution consists of the same fields as the task series, except there are no fields to make the task recurring.
4. Click 'Save' to create the on-event control task.
5. Close the tab, open and refresh the control execution tab (showing 'All control executions'). This task is now visible in the task overview. Highlight the on-event task.

## Task Workspace for Responsible

This section describes how a responsible user interacts with control execution tasks.

The responsible user can view and open control execution tasks using their personal calendar. The task is marked as an all-day event. Alternatively, the responsible can use the task workspace, which provides an overview of all tasks and can be used by responsibles, reviewers, and control writers to monitor tasks.

To open and execute a task as a responsible:

1. Login as a control execution responsible.
2. Go to the calendar and highlight the task, or navigate to the task workspace.![](<../../../.gitbook/assets/image (7).png>)
3. Open the task from the workspace. A new tab will open showing the details page of the task.
4. The task will initially be in the 'To do' status.
5. On the left navigation panel, you can:
   * See the linked controls.
   * Add and view documents.
   * Add and view hyperlinks.
   * See the task history.
6. To execute the control task, go back to the details page.
7. Add the evidence.
8. Fill in the score (e.g., select 'Effective').
9. Write a comment.
10. You can save your work using the save button and complete it later.
11. When you are ready, click on the 'Mark as done' button.\
    ![](<../../../.gitbook/assets/image (8).png>)
12. The responsible has now completed the task.

## Task Workspace for Reviewer

This section outlines the process for reviewing control execution tasks.

If a reviewer has been selected for a task, they will receive an email to review it.

To review a task:

1. Login with the user linked as a reviewer.
2. Open the email link or navigate directly to the task.
3. The task will open and its status will be 'Ready for review'.
4. The reviewer has read-only rights and can only reject or accept the task.\
   ![](<../../../.gitbook/assets/image (9).png>)
5. **If rejecting the task:** The status of the task will change to 'rejected', and the responsible will be notified by email. The responsible must then execute/update the task again.
6. **To accept the task:**
   * Click on 'Accept'.
   * Fill in a comment.
7. The status of the task will change to 'done', and the responsible will be notified by email that the task has been accepted by the reviewer.
8. The reviewer has the option to reopen the task. If the task is reopened, it will revert one step back in the workflow to be handled by the reviewer. The responsible will also be informed by email that the task has been re-opened.
9. In a scenario where no reviewer has been selected for the task, the responsible can reopen the task if needed.

