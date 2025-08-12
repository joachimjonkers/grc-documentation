# Budget-based Risk Scoring

## Preparations for Using Risk Budgets

Preparations start from a dashboard that includes the **Administration Controls** widget, which is available for an unrestricted administrative user.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Set the Application Settings to Budget-Based Risk Scoring

#### Steps to take:

1. As an administrator, go to the **Administration Controls** section of the dashboard and select **Environmental Settings**.
2.  Select **Risks** in the left menu and activate the **5th toggle: Use Budget-Based Risk Scoring**.

    <figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>
3. **Do not** use the setting **“Show Risk Quantitative Scoring Details”** (this will display extra details, which might be confusing if budget-based risk scoring is used as well).
4. Restart the application by pressing **Ctrl + F5** or **Ctrl + R**.

### Define Risk Scales Including Financial Impact and Likelihood

#### Steps to take:

1.  As an administrator, go to the **Administration Controls** section of the dashboard and select **Standing Data**. The menu shows a screen with this set up (without values):

    <figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>
2. Go to **Risk > Risk Scores > Risk Financial Impact**.
   * Five score options are predefined.
   * Each option can contain an explanation via the field **“Name”**, e.g., "1. Very low (less than 5%)" or "3. Moderate (between 20%-30%)".
   * For each score, a range can be given in **Min%** and **Max%**.
   * **Note**: The financial impact score is calculated only for defined ranges. If there is overlap, the highest score is chosen. Ranges should be contiguous or slightly overlapping. The **Min%** of the lowest range and the **Max%** of the highest range can remain undefined.
3. Go to **Risk Likelihood**: Define likelihood ranges in a similar manner (e.g., **1%-5%, 5%-10%**, etc.). Ensure the complete range from **1%-100%** is covered.
4. Go to **Risk Impact Scales**: Define alternative impact scales such as **Reputation** or **Quality**.
   * Click **+ ADD**.
   * Give the scale a name.
   * Enter the required scores.
   * Add a qualification to each score.

### Define Budget per Organization

Defining a budget for an organization is a new functionality available only for administrative users.

#### Steps to take:

1. As an administrator, go to the **Administration Controls** section of the dashboard and select **Organizational Budget** (after restart if settings have changed).
2. Two columns are displayed:
   * The first contains an overview of the internal organization as defined in CERRIX (**Admin Module > Standing Data**).
   *   The second column is used to define budgets per department.

       <figure><img src="../../../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>
3. After defining the budgets, press **Save**.

## Risk Budget-Based Scoring

### Score the Risk Financial Impact

#### Steps to take:

1. Choose a risk of an organization with a budget.
   1. In the risks, the budget that's shown is associated with the organization for which the risk is defined.
2. Enter the **Gross Likelihood**.
3. Enter the **Gross Financial Impact** in Euros.

The **Financial Impact Scale** will be automatically calculated based on the given budget.

#### Example:

* Organization budget: **€800**.
* Gross financial impact: **€500** (60% of budget → **Score 5: Catastrophic (>40%)**).
* Net financial impact: **€300** (37.5% of budget → **Score 4: Significant (20%-40%)**).
* **Final Financial Impact Score:** **4. Significant (20%-40%)**.

<figure><img src="../../../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Potential Loss Calculation:

* Gross financial impact: **€500**.
* Min & max gross likelihood: **10% - 20%**.
* **Potential Gross Minimum Loss:** **€50**.
* **Potential Gross Maximum Loss:** **€100**.

### Score the Overall Risk Impact

The overall gross impact score can be entered manually.

* The overall score is checked against **leading impact scales**.
* If no **leading impact scale** is selected, it will be checked against all impact scales.
* If the **leading impact scale** or the **max impact scale** do not match, a warning is displayed.
* If the warning is clicked, the **overall impact** is adjusted.

### Risk Workspace

If the budget-based risk scoring is active, in the workspace the Gross and Net financial impact is shown per risk.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

