# Process Management

{% hint style="info" %}
While we work on creating content for this documentation, more information can be found in the document below.
{% endhint %}

{% file src="../../.gitbook/assets/CERRIX Manual - Process Management.pdf" %}

## Print Functionality in Process Management

The print feature allows users to generate customized PDF exports of a process. When clicking the print icon, you can choose from the following three options, each offering different levels of detail and context:

<figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

### Print Graph

This option includes:

* Process Details
* Process Graph
* Process Steps

Use this to generate a clean and focused printout of the process without additional risk or control elements.

### Print Graph, Risks, Controls, Events, and MoIs

This version extends the standard graph with related governance data. It includes:

* All items from CERRIX (Risks, Controls, Events, and Moments of Insight) linked to the Business Dimension.
* These items are visualized in the printout, and if a Risk or Control is represented (e.g., as a floating symbol), it is considered linked—regardless of where it appears.

The section “Not linked to a process step” will only show items that:

* Are linked to the Business Dimension
* But do not appear anywhere in the printout, either connected to a step or visualized separately.

{% hint style="warning" %}
Important: The system does not analyze the position or logic of the elements—presence of the item symbol in the print is sufficient to count it as “linked”.
{% endhint %}

### Print Graph with Linked Risks and Controls

This option prints strictly what’s linked within the process graph.

Risks and Controls that are: linked to a Risk or Control symbol in the graph and that symbol is not linked to any process step are shown under the “Not linked to a process step” section.

{% hint style="warning" %}
Important: This option does not look outside the process graph. It does not include other Risks or Controls from CERRIX that may be linked to the Business Dimension but are not visually linked via a symbol in the graph.
{% endhint %}
