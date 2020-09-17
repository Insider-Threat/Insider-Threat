#**DLP Enforcement**

ID: T1000

Tactic: Proactive Messures

Platform: Linux / Mac / Mobile / Windows

Permissions Required: Standard

Data Sources: Tools

Version: 1.0

Created: 04/28/2020

Last Modified: 04/28/2020


**Overview:**
Data Loss Prevention (DLP) tools assist with detecting when sensitive information, like Intellectual Property (example: Source Code) or Personal Identifiable Information (PII)(example: Name, Date of Birth, Drivers License #), is being transferred. 

**Procedure Examples:**
Data Loss Prevention tools are used to monitor for sensitive data transfers, this can include company Intellectual Property or PII information. These tools monitor files for specific criteria and sends an Alert to the SOC team when a match is found. When an Alert is received the SOC Team will begin an investigation to validate the Alert. 

Example Scenario:

An employee is working on a project needs to send a file to a 3rd party. The DLP tool scans the file and finds that there is Source Code found inside, this will create an Alert for the SOC team and they will begin an investigation to validate the alert. 

Mitigations
1. By blocking or preventing the data transfer when the DLP tool has a detection.
2. By displaying a pop-up message, to inform the employee, that the DLP tool has detected something within their data transfer that may be sensitive and allow them to stop the data transfer. 



**Mitigations**

**Groups Applied To:**
| Group Name | Monitoring (Yes/No) |
| :---: | :---:|
| R&D	| Yes/No |
| Sales | |
| Executives and Executive Assistants |	Yes/No |
| IT Operations/InfoSec	| Yes/No |
|Support Staff/Everyone Else | Yes/No|

**Detection**
| Name | Description | Link | Risk Score |
| :---: | :---:|:---: | :---:|
|  | | | |  





