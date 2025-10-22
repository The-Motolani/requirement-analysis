# Requirement Analysis in Software Development.

## Objectives

To give a clear understanding of what the system should do and how it should perform.

## What is Requirement Analysis?

Requirements Analysis is a vital stage in the Software Development Lifecycle (SDLC) where the project team systematically collects, examines, and defines the needs and expectations for the software product. It serves to establish a shared and precise understanding among all stakeholders about what the system must achieve and the standards by which it should operate, ensuring that development aligns with business goals and user needs.

## Why is Requirement Analysis Important?

- Prevents scope creep.

- Ensures alignment with stakeholder needs

- Reduces costs and rework by catching issues early

- Provides a foundation for design, development, and testing

## Key Activities in Requirement Analysis.

- ### Requirement Gathering 🗂️

The process of collecting information from stakeholders to understand their needs and expectations.

- **Interviews**: Conduct one-on-one or group interviews with stakeholders to gather in-depth insights.

- **Surveys/Questionnaires**: Use surveys to collect feedback and requirements from a broader audience.

- **Workshops**: Facilitate collaborative workshops with stakeholders to discuss needs and align priorities.

- **Observation**: Observe end-users in their work environment to understand their challenges and workflows.

- **Document Analysis**: Review existing documentation, reports, or system specifications to identify current functionalities and gaps.

### - Requirement Elicitation ✍️

The process of extracting, clarifying, and refining requirements through active engagement with stakeholders.

- **Brainstorming**: Organize creative sessions to generate ideas and explore potential features.

- **Focus Groups**: Conduct focus group discussions to gather detailed feedback and validate requirements.

- **Prototyping**: Develop mockups or prototypes to help stakeholders visualize the system and refine expectations.

### + Requirement Documentation 📚

The formal recording of gathered and elicited requirements for clear communication and reference.

- **Requirement Specification Document**: Create a comprehensive document outlining all functional and non-functional requirements.

- **User Stories**: Write user stories to represent functionalities from the end-user’s perspective.

- **Use Cases**: Develop use case diagrams to illustrate how users will interact with the system.

### - Requirement Analysis and Modeling 📊

The process of examining, prioritizing, and representing requirements to ensure feasibility and alignment.

- **Requirement Prioritization**: Rank requirements based on their business value, urgency, and impact.

- **Feasibility Analysis**: Evaluate each requirement’s technical, financial, and time-related feasibility.

- **Modeling**: Use visual models such as Data Flow Diagrams (DFDs) or Entity-Relationship Diagrams (ERDs) to analyze system behavior and relationships.

### - Requirement Validation ✅

The process of confirming that the documented requirements accurately reflect stakeholder intentions.

- **Review and Approval**: Present requirements to stakeholders for validation and formal approval.

- **Acceptance Criteria**: Define measurable acceptance standards for each requirement.

- **Traceability**: Create a traceability matrix to map requirements throughout development and testing, ensuring completeness and alignment.

## Types of Requirements.

### Functional Requirements

**Definition:**
Functional requirements describe what the system must do — the specific behaviours, features, and operations the software must perform. They capture the functional needs of users, stakeholders, and the system itself.

**Examples for the booking-management project** (based on the case study [Hotel booking apps like Airbnb, OYO, Booking.com.](https://medium.com/nerd-for-tech/system-design-architecture-for-hotel-booking-apps-like-airbnb-oyo-6efb4f4dddd7)) :

> “Users shall be able to search for available hotels by location, date-range and number of guests.”

> “The system shall allow users to view hotel and room details (room types, pricing, amenities, availability).”

> “The system shall allow a user to initiate a booking (select hotel & room type, submit booking request, payment integration).”

> “Hosts (hotel managers) shall be able to manage hotel listings: add/edit hotel information, room inventory, images.”

> “The system shall allow users to view and manage their bookings (see upcoming stays, past stays, cancel/reschedule where permitted).”

> “The system shall send notification (email/push) to user and hotel manager upon booking confirmation.”

### Non-Functional Requirements

**Definition:**
Non-functional requirements describe how the system must perform — the quality attributes, constraints, and external characteristics (such as performance, security, usability) that the system must satisfy.

**Examples for the booking-management project** (inspired by the case study) 

+ Performance/Latency: The system should respond to search queries under a defined time (e.g., search results should be returned in under 500 ms).

+ Scalability/Availability: The system should scale to support large numbers of concurrent users and high read/write traffic (e.g., during peak booking periods).

+ Consistency: Once a room is booked, it must immediately reflect unavailable in search results to avoid double-booking.

+ Reliability/Fault-Tolerance: The system should tolerate failures (e.g., of individual services or database nodes) with minimal disruption to users.

+ Security: The system must protect sensitive user and payment data (encryption in transit/at rest), ensure authentication/authorization for host- and user-operations.

+ Usability: The user interface (both web and mobile) should be intuitive, enabling users to complete bookings with minimal friction.
