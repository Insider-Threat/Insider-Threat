# **Anomalous Timekeeping Activity**

ID: IT1035

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email / Timekeeping Systems

Version: 1.1

Created: 04/28/2020

Last Modified: 01/27/2025

---

## **Overview:**

Hourly employees or contractors often submit timecards or reports detailing the hours worked. Fraudulent or anomalous time reporting, such as inflating overtime hours, collusion in time approvals, or claiming hours not worked, can result in financial losses and reputational risks for the company. This behavior, especially when prolonged, can significantly impact the company’s bottom line and undermine trust. 

---

## **Example Scenario:**

| **Name**                          | **Description**                                                                                      |
|-----------------------------------|------------------------------------------------------------------------------------------------------|
| **Fraudulent Time Card Submission** | An employee or contractor falsely claims 20 hours of overtime during a pay period, knowing they did not work the additional hours. Over several months, this fraudulent activity results in substantial financial losses for the company. |
| **Collusion in Time Reporting**    | Two employees agree to approve each other’s exaggerated timecards, inflating overtime hours to increase their earnings. |
| **Unusual Patterns of Overtime**   | An employee consistently logs significant overtime hours at times when no work-related activity is observed, such as during weekends or holidays. |

---

## **Mitigations**

1. Monitor timekeeping systems for anomalies, such as excessive overtime or patterns inconsistent with operational needs.  
2. Require management approval and review of all submitted timecards or reports, ensuring transparency and accountability.  
3. Implement automated timekeeping systems with built-in controls to flag unusual or excessive overtime entries.  
4. Conduct regular audits of timecards, comparing submitted hours to observed activity, such as network or application usage logs.  
5. Establish clear policies defining acceptable overtime practices and educate employees and contractors on the consequences of time reporting fraud.  

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

| **Name**                       | **Description**                                                                                 | **Link**          | **Risk Score** |
|--------------------------------|-------------------------------------------------------------------------------------------------|-------------------|:--------------:|
| Timecard Anomaly Alert         | Flags submissions with unusually high or excessive overtime hours compared to departmental norms. | [Example Link](#) | Medium         |
| No Corresponding Activity Alert | Detects discrepancies between reported work hours and observed activity, such as application or network usage. | [Example Link](#) | High           |
| Repeated Overtime Alert        | Identifies patterns of consistent overtime submissions that deviate from normal work trends.      | [Example Link](#) | Medium         |


