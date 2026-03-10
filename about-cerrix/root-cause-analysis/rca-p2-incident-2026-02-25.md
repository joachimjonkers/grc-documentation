# RCA P2 Incident 2026-02-25

### Incident Summary

**Product:** CERRIX Platform

**Date:** 2026-02-25

**Reference ID:** RCA-20260225-P2-ControlsWorkspace

### Incident Timeline

| Timestamp              | Event                                                                                        |
| ---------------------- | -------------------------------------------------------------------------------------------- |
| 2026-02-25 09:30       | Performance issues detected in the Controls workspace via internal monitoring                |
| 2026-02-25 09:52       | First customer report received, intake completed within 10 minutes                           |
| 2026-02-25 10:37       | First communication sent to affected customers                                               |
| 2026-02-25 17:27       | Second communication sent with investigation update and remediation plan                     |
| 2026-02-26 14:34       | Third communication sent confirming the fix and planned deployment schedule                  |
| 2026-02-27 02:00–05:00 | Fix successfully deployed to all production environments during scheduled maintenance window |
| 2026-02-27 09:18       | Final communication sent confirming resolution and restored stability                        |

### Root Cause

#### Root Cause

The incident was caused by a performance regression introduced in the latest release, which affected the Controls module. A change to an underlying software component altered how certain database queries were generated, resulting in significantly slower query execution for customers with larger datasets. This caused the Controls workspace to time out and fail to load for a limited number of affected environments.

#### Detection Gaps

Internal monitoring detected the issue shortly after the release was deployed. Detection and initial investigation were swift once the first symptoms appeared.

#### Reason the Issue Was Not Identified Before Release

The release was tested both functionally and on performance prior to deployment. However, the performance testing environment did not fully reflect the data volumes present in all customer environments, which meant the specific conditions triggering the issue were not reproduced during pre-release validation.

### Impact Analysis

Only select customer environments were affected. The Controls workspace was temporarily unavailable for these customers, presenting as slow loading or failure to display data. No data loss or security issues occurred. All other modules and environments remained fully operational.

The deployment of the fix required a planned maintenance window on 27 February between 2:00 and 6:00 AM CET, during which up to 30 minutes of downtime was expected.

### Resolution & Recovery Steps

#### Short-term fixes implemented

The development team identified and resolved the inefficient query responsible for the timeouts. A targeted fix was developed, tested, and validated before being deployed to all affected production environments during a controlled maintenance window.

#### Confirmation of stability

After deployment, the Controls module was validated against production data to confirm that performance had returned to expected levels. Monitoring tools were used to verify query execution times and error rates. Additionally, confirmation was received from affected customers that the Controls workspace was loading correctly.

### Lessons Learned

#### What worked well

Internal monitoring enabled early detection of the issue. Cross-team collaboration between Development and Product (Support) was effective, and customers were proactively informed throughout the process with regular updates.

#### What didn't work well

Communication around the deployment timeline could have been more consistent. The initially communicated schedule was adjusted, and this change was not explicitly acknowledged in subsequent customer updates.

#### Preventive & Corrective Actions

To prevent similar incidents in the future and further strengthen our service reliability, we are taking the following actions:

| Action                                                                                                                       | Due date   |
| ---------------------------------------------------------------------------------------------------------------------------- | ---------- |
| Investigate adding performance and query validation checks to our automated testing pipeline                                 | 2026-06-01 |
| Formalize our incident response process, including communication guidelines and templates                                    | 2026-06-01 |
| Ensure the performance testing environment is representative of customer environments in terms of data volume and complexity | 2027-01-01 |

We remain fully committed to continuously improving our processes and minimizing any potential impact on our customers. Thank you for your understanding and trust.

If you have any questions about this Root Cause Analysis, please reach out to us: [getting-support](../getting-support/ "mention")
