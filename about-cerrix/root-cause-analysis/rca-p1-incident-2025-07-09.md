# RCA P1 Incident 2025-07-09

## Incident Summary

**Product:** CERRIX Platform

**Date:** 2025-07-09

**Reference ID:** RCA-20250709-P1-ReleaseDowntime

## Incident Timeline

<table><thead><tr><th width="178.72265625">Timestamp</th><th>Event</th></tr></thead><tbody><tr><td>2025-07-08 22:00</td><td>Opening of release window of sprint 46 and sprint 23 to all production environments</td></tr><tr><td>2025-07-08 22:13</td><td>Downtime starts for first customer environment</td></tr><tr><td>2025-07-08 23:59</td><td>All customer environments unavailable</td></tr><tr><td>2025-07-09 07:20</td><td>Detection that the production environments not available</td></tr><tr><td>2025-07-09 07:30</td><td>Requeued the release for all production environments</td></tr><tr><td>2025-07-09 08:00</td><td>Customer environments starting to become available again one by one</td></tr><tr><td>2025-07-09 08:45</td><td>Mail sent to all customers informing them of the downtime</td></tr><tr><td>2025-07-09 09:37</td><td>All production environments up and running except for the incidents module</td></tr><tr><td>2025-07-09 11:00</td><td>All production environments up and running including the incidents module</td></tr></tbody></table>

## Root Cause

### Root Cause

The incident was caused by a configuration error related to deployment permissions. As a safety measure, the environments were automatically shut down to prevent further issues and required manual intervention to restore service.

### Detection Gaps

Although monitoring and alerting systems functioned as designed, the alerts were not noticed by the responsibles at time of deployment.

### Reason the Issue Was Not Identified Before Release

The incident was not related to the code changes deployed, but rather to the deployment configuration itself. As a result, it was not identified during pre-release testing or acceptance testing.

## Impact Analysis

Customers have experienced 8.5-11 hours downtime in all their production environments, mostly outside of business hours. The environments were not accessible, instead they provided the customer with an error page, making it impossible for them to log in.

The release concerned the production environments only, all their test and acceptance environments have been up and running without any issues.&#x20;

## Resolution & Recovery Steps

### Short-term fixes implemented

A new deployment was executed on PRD for all environments, with the correct configuration.

### Confirmation of stability

Confirmation from customers, monitoring on environments, health check and smoke testing on internal production environments, all took place in order to make sure that the environments are back to normal.

## Lessons Learned

### What worked well

The communication was handled by the Product Team and Consultancy with great care. The time between time of detection and time of resolution was quite fast.

### What didn’t work well

One of the main issues highlighted by this incident, is the fact that for the time when the incident took place, the alerting did not notify a member of the team when manual intervention was required for the update to be completed.&#x20;

### Preventive & Corrective Actions

To prevent similar incidents in the future and further strengthen our service reliability, we are taking the following actions:

<table><thead><tr><th width="515.32421875">Action</th><th>Due date</th></tr></thead><tbody><tr><td>We will review and improve our release configurations to prevent this specific issue from occurring again in future deployments.</td><td>2025-07-14</td></tr><tr><td>We are enhancing our release tooling to allow for more streamlined and reliable requeuing of releases, ensuring smoother and faster resolution in case of unexpected issues.</td><td>2025-08-04</td></tr><tr><td>In addition, we are providing further training and knowledge sharing to ensure that senior team members are fully up to speed with all aspects of the release process.</td><td>2025-07-14</td></tr><tr><td>Finally, we are revising our release planning and support structure to ensure that technical support is always available during release windows, including outside regular business hours when needed.</td><td>2025-08-04 (before the next PRD release)</td></tr></tbody></table>

We remain fully committed to continuously improving our processes and minimizing any potential impact on our customers. Thank you for your understanding and trust.

If you have any questions about this Root Cause Analysis, please [get in touch with us](../getting-support.md).
