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

{% hint style="info" %}
Did you know you can use Control Execution Tasks as evidence for Control Advanced Effectiveness Testing? Read more [here](../control-advanced-effectiveness-testing/execution-based-control-testing.md).
{% endhint %}

## Activating Control Execution for a Control

To start using control execution tasks, you must first activate control execution for the relevant control:

1. Go to the Controls module.
2. Select the control you want to enable execution for.
3. Enable the Control Execution toggle (see screenshot below).
4. Save the changes.
5. After saving, 'Control execution' button will appear in the upper right corner of the screen.

<figure><img src="../../../.gitbook/assets/Screenshot 2026-02-10 112709.png" alt="Toggle:" width="375"><figcaption></figcaption></figure>

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
   * **Task Score Options:**&#x20;
     * Required: The score must be given by either Responsible or Reviewer before the task can be finished. (Reviewer only in those case where a reviewer is defined)
     * Optional: score can be given, but is not mandatory
     * Task score not visible: scoring is not part of this task execution evaluation

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

5. Navigate to the end of the page to plan the control task series.
6. Select the frequency for the recurring task:
   * When **Repeat Yearly** is selected, the user can configure:
     * **Repeat every:** number of years (e.g., 1 year)
     *   **Repeat on:**

         **Month** (e.g., February), and either:

         * **Day** of the month (e.g., 15th), or
         * **Weekday** (e.g., First Monday)
   * When **Repeat Monthly** is selected, the user can configure:
     * **Repeat every:** number of months (e.g., 3 months)
     * **Repeat on:**
       * **Day** of the month (e.g., 10th), **or**
       * **Weekday** (e.g., First Tuesday), **or**
       * **Workday** (e.g., 5th Workday skipping weekends and holidays), _if workdays and holidays were defined in the **Workday Organizer** module in the Administration Controls. \*If the chosen work day doesn’t exist in a month, the task is scheduled on the last working day of that month._
   * When **Repeat Weekly** is selected, the user can configure:
     * **Repeat every:** number of weeks (e.g., 2 weeks)
     * **Repeat on:** select one or more days of the week (e.g., Monday)
   *   **Daily tasks (using Weekly mode)**

       If a user wants to create a **Daily** recurring task:

       * Set **Repeat Weekly**
       * Set **Repeat every:** 1
       * Select **all days of the week** under **Repeat on**
7. Fill in the **Start date** (e.g., 1 January 2025) and **End date** (e.g., 31 December 2025) for the task series.
8. Click 'Save' to create the task series.
9. After the page refreshes, the task series will be created based on the selected frequency. Only the end date can now be changed.
10. Close the task series tab and refresh the control execution screen to get an overview of the created task series. The task series that was just created will be shown in the section "All control executions" .
11. Open 'Recent and upcoming' to view the 8 unfinished tasks with the earliest action date and the last 5 tasks finished .

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
11. When you are ready, click on the 'Mark as done' button. In those tasks where a Reviewer is added, the button is called "Ready for review".\
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
5. **To Reject the task:**&#x20;

* Click on "Reject" button
* Writing a comment is required

The status of the task will change to 'rejected', The responsible will be notified by email. The comment will be added in the mail and will show above the task to be redone by the responsible.

6. **To Accept the task:**

* Click on "Accept" button
* Writing a comment is optional

The status of the task will change to 'done', and the responsible will be notified by email that the task has been accepted by the reviewer, the comment (if there's one) will display above the task.

7. The reviewer has the option to reopen the task. If the task is reopened, it will revert one step back in the workflow to be handled by the reviewer. Comment is required when reopening. The responsible will also be informed by email that the task has been re-opened.
8. In a scenario where no reviewer has been selected for the task, the responsible can reopen the task if needed.

