
# Report and Presentation

## 5 Report and Presentation
COIT20246 Project Part 2: Report
Title: Network & Cybersecurity Design and Evaluation for Travel Agency
Authors:
Student 1: Prathyusha Birdar
Student 2:  Surya Prathap V

1. Cloud Services Evaluation
## 1.1 Cloud VM Specifications (Standardised across providers)
The evaluated virtual machines for cloud providers have consistent configurations, featuring Ubuntu 20.04 LTS Linux OS, 2 vCPUs, 8 GB of RAM, and 50 GB of temporary disk space. They are designated to operate in the Australia East / Sydney region, with an expected usage of 730 hours per month over a three-year timeframe.
## 1.2 Cloud Provider 1: Microsoft Azure
The Microsoft Azure D2 v3 virtual machine was assessed. It is expected to cost about USD 0.125 per hour, which totals roughly USD 91.25 each month. Over a period of three years, the combined cost for four servers is estimated to be approximately USD 13,140.
## 1.3 Cloud Provider 2: Google Cloud Platform (GCP)
Google Cloud Platform (GCP) provides the n4-standard-2 virtual machine, which costs roughly USD 87.48 per month. Over a three-year period, the total expense for four servers is estimated to be around USD 12,597.
## 1.4 Recommendation
Google Cloud Platform (GCP) is the preferred cloud provider due to its better cost efficiency over three years. Additionally, it offers dependable uptime and availability in Australia, smooth integration with backup and redundancy services, and strict compliance with Australian data locality regulations.
## 2. Security Risk Assessment
## 2.1 Identified Threats and Assets
The essential data assets designated for safeguarding include CRM systems, payroll data, travel booking details, and email archives. Significant network infrastructure components consist of the core router, server rack, and switches.
## 2.2 Summary Risk Matrix (from TVAMatrix)
A summary risk matrix highlights various threats along with their likelihood, impact, and resulting risk levels:
The following figure illustrates that
 
## 3. Recommended Security Controls
Security controls are crucial measures put in place to protect data, systems, and networks from potential risks. They serve different purposes: some are preventive, aiming to stop incidents before they happen; others are detective, designed to identify threats as they occur; and some are corrective, focused on reducing damage after an incident has taken place.


## 3.1 Control 1: Multi-Factor Authentication (MFA)
Implementing Multi-Factor Authentication (MFA) is recommended for all employees accessing essential systems such as CRM, Payroll, and other internal platforms. This security measure greatly decreases the likelihood of unauthorized access caused by phishing attacks or the reuse of compromised passwords. MFA can be deployed using tools like Azure AD MFA or Google Authenticator. It should be applied at the CRM Web Access Portal, securing both cloud-based and on-site access points. While MFA enhances security, it may also cause inconvenience for users due to extra login steps and could require additional support and training for staff.

## 3.2 Control 2: Network Segmentation
Network segmentation is advised for safeguarding vital systems like CRM, HR, and travel booking platforms. Its main purpose is to reduce the chance of malware or insider threats spreading laterally within the network. This is achieved through VLAN-based separation and the application of Access Control Lists (ACLs). These security measures are typically implemented at the distribution layer on switches and integrated into firewalls.

## 3.3 Control 3: Data Backup and Disaster Recovery Plan
A comprehensive Data Backup and Disaster Recovery Plan is essential for CRM databases and server setups. It helps protect against data loss caused by ransomware or malicious acts. The plan includes daily encrypted cloud backups, possibly using GCP Buckets with lifecycle management, as well as automated snapshot scripts. These backups are stored securely in cloud storage.
## 4. Ethical & Privacy Considerations
This section examines the ethical issues pertinent to the scenario.

## 4.1 Collected Data:
The organization gathers different kinds of data, such as customer travel details, passport or ID documents, payment information, and personal communications like emails and tickets. A major issue is that organizations frequently collect this data without adequately informing users or securing explicit consent. Additionally, the widespread use of surveillance and tracking tools like cookies, GPS, and social media monitoring extensively observe user activities, leading to serious privacy worries.
## 4.2 Risks:
Risks involve the exposure of sensitive information, potentially resulting in identity theft and financial harm to customers. The organization may also face legal consequences for failing to adhere to data protection laws. There is a danger of data misuse, such as biased profiling or targeted manipulation in advertising. Furthermore, cyber threats like phishing, ransomware, and malware attacks threaten data theft and damage.
## 4.3 Regulations:
Various regulations oversee data privacy and security, such as Australia's Privacy Act 1988, the European Union's GDPR, and PCI-DSS standards for credit card data. Additionally, HIPAA in the United States safeguards health information, and certain countries have data localization laws that mandate storing data within specific national boundaries.
## 4.4 Mitigation:
Mitigation efforts include deploying encryption methods such as TLS/SSL and AES-256, obtaining user consent, and performing frequent security assessments and staff training. For individuals, recommended practices are creating strong, unique passwords, enabling two-factor authentication, avoiding the sharing of personal details online, and staying vigilant against phishing attempts. Organizations should focus on keeping software up to date, conducting regular security reviews, and establishing clear, transparent privacy policies.
5. Project Reflection
## 5.1 GitHub Contribution ()
A screenshot illustrating the GitHub commits is provided. It notes that "GhubU121" refers to Surya Velisetti, although the name may not always accurately reflect in the display.


## 5.2 Task Division:
The division of tasks between the two students (Student A :Prathyusha Birdar and Student B: Surya Prathap V) was as follows:


## 5.3 Collaboration Review
Student 1 (Prathyusha Birdar) made 35 Git commits, whereas Student 2 (Surya Prathp V) made 28. The number of commits largely reflected the tasks assigned. Both students contributed commits in 7 of the 10 weeks of the project.
5.4 Reflection
Successful teamwork was supported through weekly meetings, shared Google Docs, and smooth integration between VS Code and GitHub. A key obstacle faced was an early difficulty in understanding cloud cost estimators. For future efforts, recommendations include beginning projects sooner, reviewing unit tools more promptly, and setting more rigid deadlines.


### 5.2 Recorded Presentation
The presentation will be a recorded video that must cover the following:
1. Explain briefly the key ethical issues that the organisation must consider, with each student 
explaining one issue. (Section 4.4)
2. A summary of who contributed to the different tasks during the project, and how many Git 
commits each student made. (Section 4.5)
3. A summary of how your group worked together, e.g., how often you met, where did you meet (inclass, after class, online), what communication mechanisms you used. (Section 4.5)
4. Reflection on what went wrong and how you can improve in the future. (Section 4.5)

The presentation must meet the following requirements:
- All students in the group must speak, e.g., take in terms covering the different parts.
- On the first appearance, each speaker must identify themselves before presenting. This includes 
showing the speaker’s face on the screen (either full screen or in thumbnail).
- No PowerPoint slides are needed. You are recommended to speak without notes. You may show 
parts of your report on the screen if relevant but should not be reading your report.
- Duration of approximately 5 minutes (about 1 minute for each of the items). The duration must be 
more than 4 minutes and less than 7 minutes.
- The presentation should be submitted as a single file. The file format must be mp4.
