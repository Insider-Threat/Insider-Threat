# **Printing**

ID: IT1028

Tactic: Exfiltration

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Admin

Data Sources: Application / Authentication / Endpoint / Network / Tools / Email

Version: 1.0

Created: 04/28/2020

Last Modified: 04/28/2020


## **Overview:**
Copy machines and printers are widely used across many companies and have been mostly ignored by security monitoring tools. These devices can often allow a user to avoid Data Loss Prevention (DLP) tools or other restrictions by accessing documents that were printed and/or copied by other users. A user might also avoid detection by printing out sensitive documents that they have direct access to, again possibly avoiding DLP tools or other restrictions. 
## **Example Scenario:**

| Name | Description |
| :---:| :---:|
| Data Exfiltration Via Printer | A user is about to leave the Company, before their last day, the user decides they would like to take technical details of a project they are working on. Worried they will lose access to the work they have created, the user prints out all of the project data they have.       |
| Sensitive/Confidential Discovery and Exfiltration| A user connects to an offices shared Copier/Printer, from there they can view previous "jobs" that the device has stored that they would not otherwise have access to. From this queue, the user is able to find a sensitive document that a Vice President recently printed out containing a list of customers and how much they are spending on certain products. The user is then able to also print the sensitive file from themself.  

## **Mitigations**
1. Ensuring proper configurations of Copy/Printers. 
2. Monitoring printer and copier activity. 





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





