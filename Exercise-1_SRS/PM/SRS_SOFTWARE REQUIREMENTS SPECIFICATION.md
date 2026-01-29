SOFTWARE REQUIREMENTS SPECIFICATION (SRS)
 Lost & Found Portal
1. Introduction: 
1.1 Purpose
This Software Requirements Specification (SRS) document describes the functional and non-functional requirements of the Lost & Found Portal system. The purpose of this document is to provide a clear and complete description of system requirements for academic evaluation under the Software Engineering and Agile Development (SEAD) course.
This document serves as a reference for project planning, system design, validation, and review.
1.2 Scope
The Lost & Found Portal system is designed to provide a centralized online platform for university students and staff to report lost and found items, search for matches, and manage claims.
The system aims to reduce administrative burden, improve lost item recovery rates, and enhance campus convenience through efficient digital tracking and matching.
1.3 Definitions, Acronyms, and Abbreviations
Term	Description
LFP	Lost & Found Portal
SRS	Software Requirements Specification
UI	User Interface
Admin	System Administrator
User	Registered individual using the portal
________________________________________




2. Overall Description
2.1 Product Perspective
The system is a standalone web-based application that supports campus lost and found operations by centralizing reporting, search, and claim management.
It does not replace physical item handling but assists students, staff, and administrators by providing digital tracking and matching.
2.2 Product Functions
The major functions of the system include:
•	Reporting lost items with descriptions, categories, and images
•	Reporting found items with descriptions, categories, and images
•	Searching and filtering lost and found items
•	Matching lost items with found items based on similarity
•	Submitting and managing claims for found items
•	User registration, authentication, and account management
2.3 User Classes and Characteristics
User Class - Description
Student – Uses the system to report lost or found items and search for matches
University Staff – Uses the system occasionally to report or search for items
Administrator – Manages user accounts, item reports, and claim verification
2.4 Operating Environment
•	Web-based application
•	Accessible through modern web browsers (desktop and mobile responsive)
•	Server-side processing for item matching and notifications
________________________________________
2.5 Design and Implementation Constraints
•	Compliance with data privacy and university IT policies
•	Item images must be uploaded in supported formats (JPG, PNG)
•	Internet connectivity required for system access
•	Users must register with valid university email addresses
2.6 Assumptions and Dependencies
•	Users provide accurate and honest item descriptions
•	Uploaded images are clear and relevant to the item
•	System performance depends on server availability and database responsiveness
2.7 User Documentation
The system will provide basic on-screen instructions to guide users through registration, item reporting, search, and claim submission. No advanced technical knowledge is required to operate the system.
2.8 System Constraints
Explain:
•	Ethical use constraints (no misuse of user data)
•	Fairness in item matching and claim verification
•	Academic and resource limitations (no mobile app, no payment integration)
________________________________________
3. Functional Requirements
Each functional requirement is uniquely identified and testable.
FR-01
Description: The system shall allow users to report lost items with details such as item name, category, description, location, date, and image upload.
Priority: High
Acceptance Criteria: Lost item reports are successfully submitted and stored in the system.
FR-02
Description: The system shall allow users to report found items with details such as item name, category, description, location found, date, and image upload.
Priority: High
Acceptance Criteria: Found item reports are successfully submitted and stored in the system.
FR-03
Description: The system shall allow users to search and filter lost and found items by keywords, category, location, and date range.
Priority: High
Acceptance Criteria: Search returns accurate and relevant results.
FR-04
Description: The system shall match lost items with found items based on description, category, and location similarity.
Priority: High
Acceptance Criteria: Matching produces relevant suggestions between lost and found reports.
FR-05
Description: The system shall allow users to submit claims for found items they believe belong to them.
Priority: High
Acceptance Criteria: Claims are successfully submitted and tracked for verification.
________________________________________
FR-06
Description: The system shall display search results, item details, and match suggestions clearly to users.
Priority: Medium
Acceptance Criteria: Users can view and interact with results clearly.
________________________________________
4. Non-Functional Requirements
NFR-01 Performance
The system shall process item reports and return search results within an acceptable response time under normal load conditions.
NFR-02 Security
The system shall ensure secure handling and storage of user data and uploaded images.
NFR-03 Usability
The system shall provide an intuitive and user-friendly interface requiring minimal training.
NFR-04 Scalability
The system shall support an increasing number of users and item reports without significant performance degradation.

