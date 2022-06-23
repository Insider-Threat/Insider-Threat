# **Excessive Overtime**

ID: IT1035

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.0

Created: 04/28/2020

Last Modified: 04/28/2020


## **Overview:**
Employees that are paid an hourly rate, or contractors that bill at an hourly rate, typically will submit some form of a time card/report stating the amount of hours they worked. These time cards/reports can be manipulated to add more time than the person actually worked, resulting in the person being paid for work they did not preform.

## **Example Scenario:**

| Name | Description |
| :---:| :---:|
| Fraudulent Time Card | An employee/contractor submits that they worked 20 hours of overtime during a pay period, knowning that they did not actually work the additional hours and they will be paid for that time. This activity continues on for several months, resulting in a considerable loss to the Company. |


## **Mitigations**
1. Monitor timekeeping for unusual activity.
2. Require management review of all submitted time cards/reports.



## **Groups Applied To:**
| Group Name | Monitoring (Yes/No) |
| :---: | :---:|
| R&D	| Yes/No |
| Sales | Yes/No |
| Executives and Executive Assistants |	Yes/No |
| IT Operations/InfoSec	| Yes/No |
|Support Staff/Everyone Else | Yes/No|

## **Detection**
| Name | Description | Link | Risk Score |
| :---: | :---:|:---: | :---:|
| Name of Alert | Brief Description | Link to Alert | Risk Score|  
