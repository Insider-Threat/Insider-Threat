# **Use of File Share Site with External User**

ID: IT1040

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.0

Created: 04/28/2020

Last Modified: 04/28/2020


## **Overview:**
When a Company uses a File Sharing or Hosting Application, like Microsoft SharePoint or Box, users may have the ability to share files with others outside of the Company. A malicious Insider, may use this as an opportunity to share data with others or allow their personal account access to restricted data in an attempt to avoid detection. 

## **Example Scenario:**

| Name | Description |
| :---:| :---:|
|  Data Sharing | An employee is about to resign from the company, before they give their notice, they add one of their personal email accounts to the Company's File Share site. This allows them to download files as an external user in an attempt to conceal their activity.     |
  

## **Mitigations**

1. Monitor File Sharing Activity.
2. User Role Based Access to secure Confidential/Sensitive data.
3. Limit Confidential/Sensitive repositories to internal sharing only. 




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





