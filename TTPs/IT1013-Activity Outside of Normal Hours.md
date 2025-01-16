# **Activity Outside of Normal Hours**

ID: IT1013

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Authentication / Endpoint / Network / Tools

Version: 1.1

Created: 04/28/2020

Last Modified: 01/16/2025

---

## **Overview:**

Most employees follow predictable work patterns based on their job functions. Deviations from these behavioral norms, such as accessing systems or data during unusual hours, may indicate an insider threat. Such activity could suggest attempts to evade detection or unauthorized access to sensitive data when others are unlikely to notice. Monitoring and investigating anomalous activity during non-standard hours are critical for mitigating risks.

---

## **Example Scenario:**

| **Name**                   | **Description**                                                                                      |
|----------------------------|------------------------------------------------------------------------------------------------------|
| Employee Collecting Data   | An employee works Monday through Friday from 9 AM to 6 PM. On Sunday at 10:39 AM, the employee logs in, browses file shares, and accesses multiple files. This could indicate an attempt to avoid detection by working outside normal hours. |
| Unauthorized Weekend Activity | An employee logs in during the weekend and begins accessing project files unrelated to their current assignments, raising suspicion. |

---

## **Mitigations**

1. Restrict access to sensitive information based on time of day or day of the week using time-based access controls.  
2. Monitor logins and activity outside standard business hours, focusing on sensitive systems or data.  
3. Implement behavioral analytics tools to establish baselines for employee activity and flag anomalies.  
4. Educate employees on acceptable use policies and emphasize that working outside normal hours without justification could trigger investigations.  

---

## **Groups Applied To:**

| **Group Name**                | **Monitoring (Yes/No)** |
|--------------------------------|:----------------------:|
| R&D                            | Yes/No               |
| Sales                          | Yes/No               |
| Executives and Executive Assistants | Yes/No         |
| IT Operations/InfoSec          | Yes/No               |
| Support Staff/Everyone Else    | Yes/No               |

---

## **Detection**

| **Name**                     | **Description**                                                                                 | **Link**          | **Risk Score** |
|------------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Off-Hours Login Alert         | Flags logins occurring outside standard working hours for the employee.                        | [Example Link](#) | Medium         |
| Sensitive File Access Alert   | Detects access to sensitive files during unusual times, such as late at night or on weekends.   | [Example Link](#) | High           |
| Behavioral Anomaly Alert      | Identifies significant deviations from the user’s established activity patterns.               | [Example Link](#) | Medium         |
| Unusual System Access Alert   | Tracks access to critical systems or data outside of normal working hours.                     | [Example Link](#) | High           |
