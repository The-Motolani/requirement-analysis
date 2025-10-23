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

- ### Requirement Elicitation ✍️

The process of extracting, clarifying, and refining requirements through active engagement with stakeholders.

- **Brainstorming**: Organize creative sessions to generate ideas and explore potential features.

- **Focus Groups**: Conduct focus group discussions to gather detailed feedback and validate requirements.

- **Prototyping**: Develop mockups or prototypes to help stakeholders visualize the system and refine expectations.

- ### Requirement Documentation 📚

The formal recording of gathered and elicited requirements for clear communication and reference.

- **Requirement Specification Document**: Create a comprehensive document outlining all functional and non-functional requirements.

- **User Stories**: Write user stories to represent functionalities from the end-user’s perspective.

- **Use Cases**: Develop use case diagrams to illustrate how users will interact with the system.

- ### Requirement Analysis and Modeling 📊

The process of examining, prioritizing, and representing requirements to ensure feasibility and alignment.

- **Requirement Prioritization**: Rank requirements based on their business value, urgency, and impact.

- **Feasibility Analysis**: Evaluate each requirement’s technical, financial, and time-related feasibility.

- **Modeling**: Use visual models such as Data Flow Diagrams (DFDs) or Entity-Relationship Diagrams (ERDs) to analyze system behavior and relationships.

- ### Requirement Validation ✅

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

## Use Case Diagrams

A Use Case Diagram is a type of diagram in the Unified Modeling Language (UML) that visually illustrates the interactions between actors (users or other external systems) and the system under consideration. 

**Key elements include:**

- **Actors:** Entities external to the system (users, other systems) that initiate or are affected by interactions. 

- **Use Cases:** Represent specific goals or tasks that the system performs in response to an actor’s actions.

- **System Boundary:** Defines what is inside the system (in scope) versus what is external. 

- **Relationships:** Include, extend, and generalization relationships help model reusable behaviours or alternative flows.

### Benefits of Use Case Diagrams

Here are some of the main advantages of using use case diagrams in software development and requirements engineering:

#### Improved Communication & Shared Understanding

Use case diagrams provide a visual representation that is easier for non-technical stakeholders (like business users, product owners) to understand. They create a shared “language” between business, analysts, and developers. 

#### Clarifies System Scope and Interactions

By explicitly showing actors and system boundaries, they help teams understand what the system will do, and what lies outside its scope. This helps set clear expectations, reduce ambiguity, and avoid scope creep. 

#### Supports Requirements Gathering and Analysis

Use case diagrams help identify and organize functional requirements by showing how users interact with the system and what goals they have. This helps find missing requirements, overlaps, or inconsistencies early. 

#### Foundation for Design, Testing & Validation

- They offer input for system design: helping designers and architects understand user interactions and plan system behavior. 

- They also aid in deriving test cases: from each use case you can generate scenarios to verify the system meets its requirements.

#### Helps Manage Complexity and Reuse

Especially in larger systems, use case diagrams help break down the system into manageable parts. Also, relationships like “include” allow reuse of common functionalities across use cases.

##### Example of a Use Case Diagram
![booking system use case diagram](https://github.com/The-Motolani/requirement-analysis/blob/main/alx-booking-uc.png)
> - Source: [Creately](app.creately.com)

## Acceptance Criteria
Acceptance criteria are the specific conditions that a feature (or user story) must meet in order to be accepted by stakeholders. They focus on the “what” needs to be done (outcome) rather than the “how”.

### Importance of Acceptance Criteria In Requirement Analysis

Including well-defined acceptance criteria brings several advantages:

- Ensures shared understanding. Stakeholders, developers and testers all see the same conditions for when a feature is complete — reducing misunderstandings. 

- Provides explicit basis for testing and validation. Since acceptance criteria are testable, they guide both development (what to build) and quality assurance (what to verify). 

- Helps maintain quality and manage scope. By making what “done” means explicit, you reduce the chance of scope creep, incomplete features, and surprises. 

- Improves efficiency. Clear criteria reduce ambiguity, which means fewer revisions, quicker development, fewer misunderstandings and rework. 

- Aligns development with business value. Because they are defined from the user or stakeholder perspective they help ensure that what is built truly delivers the intended value.

### Example

**User Story:**
As a registered guest, I want to complete payment and confirm my booking so that my reservation is secured and I receive confirmation.

**Acceptance Criteria:**
**Scenario: Successful booking checkout**

- Given the guest is logged in and has selected a hotel, room type, check-in date, check-out date, and guest count

- And the guest has entered valid payment information (e.g., credit card or supported payment method)

- When the guest clicks the “Confirm Booking & Pay” button

- Then the system processes the payment successfully

- And the booking status changes to “Confirmed”

- And an email (and/or push notification) is sent to the guest within 2 minutes containing the booking reference, hotel details, stay dates, price breakdown, and cancellation policy

- And the booked room inventory is immediately updated to reflect the reservation so no double-booking occurs

**Scenario: Payment failure handling**

- Given the guest is logged in and at checkout but payment fails (e.g., card declined, funds insufficient)

- When the payment attempt is made

- Then the checkout page displays a clear error message (“Payment could not be processed – please try another method or card”)

- And the booking status remains “Pending” (not confirmed)

- And the guest remains on the checkout page with the option to retry payment or choose another payment method

**Scenario: Checkout timeout / performance requirement (non-functional)**

- Given the system is under normal load conditions

- When the guest clicks “Confirm Booking & Pay”

- Then the system displays a booking confirmation or payment error within 5 seconds

- And the guest doesn’t see any time-out error or “session expired” message within that period

**Scenario: Supported payment methods**

- Given the guest is at the payment step

- When the guest selects a payment method

- Then the system supports at least the following methods: major credit/debit cards, and one local/regional payment method (e.g., mobile money or local bank transfer)

- And the guest can complete payment using any of these methods without additional hurdles

**Scenario: Data integrity and traceability**

- Given the booking is completed (confirmed)

- Then a traceability record is created linking the guest, booking, payment transaction ID, room inventory change and notification sent

- And this record is accessible by the host/hotel manager in their dashboard and by the system admin for auditing.
