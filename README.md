# Salesforce CRM solution designed for Mfanageza Trading Projects
The solution streamlines candidate registration, compliance verification, document management, automated notifications, and reporting for SETA and SAQA programmes.
---
Mfanageza Trading & Projects CRM Solution
Project Overview
This project is a Salesforce CRM solution designed for Mfanageza Trading & Projects, a South African skills development and training company led by Bongani Mfana ka Geza.
The solution streamlines candidate registration, compliance verification, document management, automated notifications, and reporting for SETA and SAQA programmes.
Rather than being a simple Trailhead exercise, this project demonstrates a real-world Salesforce implementation focused on solving business challenges through automation, data quality, and process improvement.

Business Problem
Mfanageza Trading & Projects manages large numbers of candidates applying for skills development and training programmes.
Before this solution:
Candidate information was captured manually.
Compliance documents were difficult to track.
Staff manually followed up with candidates.
Missing or rejected documents delayed programme registration.
SETA reporting required significant manual effort.
The objective was to digitize the entire candidate compliance process using Salesforce.





Solution Architecture
Candidate (Contact)
        │
        ▼
Compliance Document
        │
        ▼
Verification Status
        │
        ▼
Salesforce Flow Automation
        │
        ▼
Automated Email Notification
        │
        ▼
Reports & Dashboards



Salesforce Objects
Contact (Candidate)
The Contact object stores candidate information, including:
First Name
Last Name
Email Address
Mobile Number
South African ID Number
Programme
Province
Compliance Document (Custom Object)
A custom object created to manage candidate compliance documentation.
Fields
Document Type
Verification Status
Rejection Reason
Upload Date
Candidate (Lookup Relationship)
Verified By
Verification Date
Relationship
Candidate
     │
     └──── Compliance Document

One candidate can have multiple compliance documents linked to their profile.


Validation Rules
A custom validation rule ensures that every South African ID Number contains exactly 13 digits before the record can be saved.
Business Value
Prevents invalid candidate records.
Improves data quality.
Supports SETA compliance.
Reduces administrative errors.


Salesforce Automation
Automated Compliance Rejection Flow
A Record-Triggered Flow automatically sends an email whenever:
Verification Status = Rejected

The candidate immediately receives a notification explaining why the document was rejected and what action is required.
Example Email
Hi Kabelo,

Thank you for submitting your compliance documents.

Your Certified ID Copy has been rejected.

Reason:
The document is unreadable.

Please upload a clearer certified copy so we can continue processing your application.

Kind Regards,

Mfanageza Trading & Projects


Email Template
Compliance Document Rejection Notice
Dynamic merge fields include:
Candidate First Name
Document Type
Rejection Reason
This eliminates the need for staff to manually send rejection emails.
Business Process Flow
Candidate submits documents
          │
          ▼
Compliance Review
          │
          ▼
Verification Status
      ┌───────────────┐
      │               │
      ▼               ▼
 Approved         Rejected
      │               │
      ▼               ▼
 Continue      Salesforce Flow
 Registration         │
                      ▼
          Automatic Email Notification
                      │
                      ▼
         Candidate uploads corrected document



Reports & Dashboards
The CRM enables management to monitor:
Compliance Documents by Status
Approved Documents
Rejected Documents
Documents Awaiting Verification
Candidates Ready for SETA Registration
Compliance Progress Dashboard

Features Implemented
Custom Candidate Management
Compliance Document Custom Object
Lookup Relationships
Validation Rules
Record-Triggered Flows
Email Templates
Automated Notifications
Salesforce Reports
Dashboard-ready Data Model


Skills Demonstrated
Salesforce Administration
Custom Objects
Custom Fields
Lookup Relationships
Page Layouts
Validation Rules
Security Configuration
Profiles
Salesforce Automation
Record-Triggered Flows
Email Automation
Business Process Automation
CRM Design
Data Modelling
Relational Database Design
Candidate Lifecycle Management
Business Process Mapping
Business Analysis
Requirements Gathering
Workflow Design
Compliance Management
Process Improvement


Business Benefits
This solution delivers measurable business value by:
Reducing manual administration.
Improving candidate onboarding.
Increasing data accuracy.
Automating compliance communication.
Improving reporting and visibility.
Creating a scalable CRM solution for future growth.

Technologies Used
Salesforce Lightning Experience
Salesforce Flow Builder
Custom Objects
Validation Rules
Email Templates
Reports & Dashboards

Future Enhancements
One-click SAQA/SETA Export Report
Candidate Self-Service Portal (Experience Cloud)
Approval Process for Compliance Verification
Power BI Executive Dashboard Integration
Digital Signatures for Training Agreements


Learning Outcomes
Through this project, I gained practical experience in:
Designing a Salesforce CRM solution from business requirements.
Creating custom Salesforce objects and relationships.
Building validation rules to improve data quality.
Automating business processes using Flow Builder.
Designing scalable CRM solutions for compliance management.
Developing reports and dashboards to support business decision-making.


About the Project
Project Name: Mfanageza Trading & Projects CRM Solution
Role: Salesforce Administrator & Business Analyst
Purpose: To design and implement a Salesforce CRM solution that manages candidate registration, compliance verification, document tracking, and automated communication for South African skills development programmes.

Screenshots
(Add screenshots of your Salesforce implementation here.)
Home Page
Contact Object
Compliance Document Object
Validation Rule
Record-Triggered Flow
Email Template
Reports
Dashboard


Author
Kabelo Gopane
Role: Salesforce Administrator | Business Analyst | CRM Enthusiast
This project forms part of my Salesforce portfolio and demonstrates my ability to design, configure, automate, and implement real-world CRM solutions that solve business challenges using Salesforce.

