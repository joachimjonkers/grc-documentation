# Execution-Based Control Testing

{% hint style="warning" %}
This functionality will be available in ACC on 31 December 2025 and in PRD on 14 January 2026.
{% endhint %}

**Execution-based control testing** allows you to assess the effectiveness of controls by directly using the control execution tasks that occurred within a defined test period. This feature integrates control execution data with advanced effectiveness testing, providing a streamlined and auditable testing workflow.

{% hint style="info" %}
Execution-based control testing is only available when using the latest _Control Advanced Effectiveness Testing_ screens. Most customers already use these screens. If your environment does not yet have them enabled, please contact [CERRIX Support](../../../about-cerrix/getting-support/).
{% endhint %}

## **Overview**

In many organizations, controls require [tasks](../controls/control-execution-tasks.md) to be executed according to a predefined schedule (e.g., monthly access right reviews). Execution-based testing collects these tasks and uses them as the test source, removing the need to manually upload population files.

All control executions scheduled within the test period are automatically included as the source for the control test.

## **Preconditions**

Before initiating an execution-based test you must ensure that control execution is enabled in the configuration of the control:

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

## **Activating Execution-Based Testing**

Execution-based testing is configured within the control test plan.

1. Create or open a control test plan.
2. Ensure the **test period** matches a period in which execution tasks are scheduled.
3. On the second page: **Sample Generation**, enable the option: **Use control execution**

![](<../../../.gitbook/assets/Unknown image>)

This activates the automatic collection of execution tasks for the test source.

## **Starting the Control Test**

Once the test period has ended, the tester can initiate the control test as usual.

Execution-based testing consists of:

1. **Source Upload & Sampling**
2. **Evidence Upload**
3. **Testing**
4. _(Optional)_ **Review**

These follow the standard CERRIX test workflow, but with additional execution-based functionality.

### Source Upload & Sampling

When execution-based testing is enabled, CERRIX automatically loads all execution tasks planned within the test period.

![A screenshot of a computer AI-generated content may be incorrect.](<../../../.gitbook/assets/Unknown image (1)>)

#### **What you will see:**

* A summary of all **execution tasks found**.
* A count of execution tasks that were **not yet completed**. (In normal scenarios, all tasks should be completed when effectiveness testing begins.)

#### **Sample generation:**

The source uploader only needs to provide the **sample size**. After sample generation, the evidence uploader can begin their work.

#### **Notes**

* The original source, an overview of all control executions for the test plan period, remains accessible through the **Source documents** section.
* Completed execution tasks included in a test sample **cannot be deleted or reopened** to safeguard audit integrity.
* If **no execution tasks** are found in the test period, CERRIX assumes the control **did not occur.** The tester can only give a final conclusion, based on that assumption. If the control did occur, with the source  evidence not being registered in control executions but elsewhere, the testplan should be recreated without the option "Use control execution".&#x20;



### Evidence Upload

The evidence uploader sees all selected samples, each corresponding to a specific control execution. For example: ![](<../../../.gitbook/assets/Unknown image (2)>)

#### **Automatic evidence linking**

If the control execution includes evidence, this evidence is automatically copied into the sample.

Linked evidence is marked with a **link icon**, indicating that it originated from a control execution rather than a manual upload. For example: ![](<../../../.gitbook/assets/Unknown image (3)>)

#### **Situations the evidence uploader may encounter**

<table><thead><tr><th width="242.46875">Situation</th><th width="142.19921875">Explanation</th><th>What the uploader can do</th></tr></thead><tbody><tr><td><strong>Control execution completed with evidence</strong></td><td>Evidence is already present</td><td>Sample is marked <em>Done</em>. Optional: add extra evidence.</td></tr><tr><td><strong>Control execution completed without evidence</strong></td><td>No evidence found</td><td>Add evidence <strong>or</strong> mark <em>No evidence</em> and provide an explanation.</td></tr><tr><td><strong>Control execution not completed</strong></td><td>Task still open</td><td>Either ask the responsible person to complete the task, upload evidence manually, or mark <em>No evidence</em> with justification.</td></tr></tbody></table>

### Testing & Reviewing

The tester and reviewer can assess samples as they normally would. Both roles can access:

* The **source document**
* The **linked control execution tasks**
* Automatically or manually uploaded evidence

#### **Additional execution-based indicators**

* A warning appears when a task is **not completed**.
* A warning appears when a task was **completed after** the evidence uploader finished their work.
* Linked evidence from execution tasks displays a **link icon**; manually uploaded evidence does not.

## **Additional Notes**

* If there are no execution tasks within the period of the control test, it is assumed that the control didn't occur. &#x20;
* Execution tasks that were **deleted or rescheduled outside the test period** before sampling took place are not included in the population. After sampling it is not possible to delete and even  rescheduling the task will not remove it from the source of the testplan.
* This mechanism ensures a fully auditable snapshot: Execution tasks used in a test **cannot be removed from the testplan after sampling**, ensuring the integrity of the sample.
