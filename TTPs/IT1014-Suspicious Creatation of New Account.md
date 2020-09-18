# **Suspicious Creatation of New Account**

ID: IT1014

Tactic: Initial Discovery

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Application / Authentication / Endpoint / Network / Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 04/28/2020


## **Overview:**
Employees that have privileged access and/or the ability to create new accounts, could create a new account prior to their departure so they are able to access the sensitive information before or after the leave the company. 

## **Example Scenario:**

| Name | Description |
| :---:| :---:|
| Employee Creating Persistence | An employee creates a new account that will allow them to access the companies environment after their user account is deactivated.  |
  

## **Mitigations**

1. Review/audit account creation or modification activity of users with the ability to do so, when they leave the company. 
2. Revoke all elevated privileges of a user when they turn in their resignation.  



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
|  | | | |  





