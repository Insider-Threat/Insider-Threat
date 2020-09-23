# **Changing Service Account Password**

ID: IT1031

Tactic: Business Impact

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.0

Created: 04/28/2020

Last Modified: 04/28/2020


## **Overview:**
Service Account are used for many purposes, one example is for an Application/Service to be able to execute the necessary commands/functions needed for it to work properly. If the password is changed and the Application/Service is not properly updated this could lead to an outage.

## **Example Scenario:**

| Name | Description |
| :---:| :---:|
| Malicious Changing of Password | A user become disgruntled and changes the password to a service account without notifying anyone or updating the Applications that use the account causing an outage this disrupts the business.  |


## **Mitigations**
1. Limit access to users that have the ability to change passwords.
2. Ensure that more than one person has admin level access to Applications/Services. 
3. Use an account/password management tool/software and provide users with role based access. 



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





