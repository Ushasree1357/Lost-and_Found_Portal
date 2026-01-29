Design Document – Design Decisions
1. Introduction
This design document outlines the key architectural and technical design decisions made during the development of the Lost & Found Portal.
The objective is to ensure usability, modularity, maintainability, and efficiency while addressing challenges in campus lost-and-found operations such as fragmented reporting, low recovery rates, and administrative overhead.
2. Design Goals
The design decisions are guided by the following goals:
•	Simplify lost-and-found reporting for students and staff
•	Improve matching accuracy between lost and found items
•	Ensure modular and maintainable system architecture
•	Support scalability for campus-wide usage
•	Maintain transparency and fairness in claim handling
3. Architectural Design Decisions
3.1 System Architecture
Decision: Adopt a modular layered architecture.
Rationale:
•	Clear separation of concerns
•	Easier maintenance and debugging
•	Independent scalability of components
Layers:
•	Presentation Layer (User Interface)
•	Application Layer (Business Logic & APIs)
•	Matching Layer (Item Comparison & Notification Logic)
•	Data Layer (Database & Storage)
3.2 Client–Server Architecture
Decision: Use a client–server model.
Rationale:
•	Centralized data storage and processing
•	Lightweight client interface accessible via browser
4. Technology Stack Decisions
4.1 Backend Technology
Decision: Use Python-based backend services.
Rationale:
•	Strong support for web frameworks (e.g., Django/Flask)
•	Rapid development and ease of integration
•	Good support for image handling and notifications
4.2 Database Choice
Decision: Use relational database (MySQL/PostgreSQL).
Rationale:
•	Structured data for users, items, and claims
•	Supports complex queries for searching and filtering
•	ACID compliance for transaction safety
4.3 Matching Strategy
Decision: Implement rule-based and keyword-based matching instead of AI-only matching.
Rationale:
•	Simpler to implement and explain
•	Lower computational requirements
•	More transparent and controllable for campus use
5. Data Design Decisions
5.1 Item Data Structure
Decision: Store lost and found items in structured tables with categories.
Rationale:
•	Consistent representation of diverse item types
•	Faster search and filtering
•	Enables reporting and analytics
5.2 Image Storage
Decision: Use cloud storage or server directory for uploaded images.
Rationale:
•	Reduces database load
•	Supports faster retrieval and display
•	Allows scalability for large numbers of uploads
6. Use Case Design Decisions
6.1 Actor Identification
Decision: Identify system actors during early design.
Actors:
•	Student
•	University Staff
•	Administrator
•	Campus Security
Rationale:
•	Defines system boundaries
•	Helps assign responsibilities and permissions
•	Simplifies use case modeling
6.2 Use Case Relationships
Decision: Use include and extend relationships.
Rationale:
•	Avoids redundancy
•	Improves clarity of functional flow
•	Encourages reuse of common functionalities
7. Security Design Decisions
7.1 Authentication and Authorization
Decision: Implement role-based access control.
Rationale:
•	Protects user privacy and item data
•	Restricts actions based on user roles
•	Enhances system security
7.2 Data Privacy
Decision: Limit contact information visibility until claim verification.
Rationale:
•	Protects user privacy
•	Prevents misuse of contact details
•	Encourages trust in the system
8. Scalability and Performance Decisions
8.1 Asynchronous Notifications
Decision: Use background processing for email notifications.
Rationale:
•	Prevents UI delays
•	Handles bulk notifications efficiently
•	Improves system responsiveness
8.2 Caching Strategy
Decision: Cache frequent searches and item listings.
Rationale:
•	Reduces database load
•	Speeds up response times
•	Improves user experience during peak usage
9. Error Handling and Logging
Decision: Implement centralized logging and exception handling.
Rationale:
•	Simplifies debugging
•	Helps monitor system performance
•	Supports auditing and maintenance
10. Future Enhancements
The design supports future improvements such as:
•	Mobile application development
•	AI-powered image recognition for items
•	SMS notifications
•	Integration with campus ID systems
11. Conclusion
The design decisions focus on building a user-friendly, secure, and efficient lost-and-found system.

