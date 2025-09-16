Of course. Here is a Product Requirements Document (PRD) for the Special Education Management System, generated from the provided project charter.

***

# Product Requirements Document: Special Education Management System

## 1. Introduction & Purpose

This document outlines the product requirements for the **Special Education Management System**, a comprehensive Progressive Web Application (PWA) designed to streamline the management of students with special educational needs. The system aims to unify fragmented processes, addressing the critical need for efficient collaboration, documentation, and progress monitoring among educational professionals, students, and families. The primary goal is to provide a single, compliant platform for managing Individualized Education Programs (IEPs), Limited English Proficiency (LEP) support, and Section 504 accommodations.

## 2. Problem Statement

Current special education management processes are disjointed and spread across multiple systems. This fragmentation leads to several critical issues:
*   **Inefficient communication** among educators, specialists, and families.
*   **Inconsistent documentation**, making it difficult to maintain accurate and compliant records.
*   **Difficulty tracking student progress** and ensuring regulatory compliance.

## 3. Goals & Success Metrics

### 3.1. Primary Objective
To create a unified platform that enables educational professionals to efficiently manage, document, and track the progress of special education students throughout their academic journey.

### 3.2. Success Metrics
The success of this product will be measured by the following key metrics:
*   **Quantitative Metrics**:
    *   A **40% reduction in documentation time** for educators.
    *   High user adoption rates.
    *   Positive compliance audit results.
    *   High user satisfaction scores.
*   **Qualitative Measures**:
    *   **Improved collaboration efficiency** between educators, specialists, and families.
    *   **Enhanced compliance tracking** and reporting capabilities.
    *   **Increased accessibility and usability** for all stakeholders.
    *   Improvements in educational outcomes.

## 4. User Personas

The system is designed to serve several key user groups with distinct needs and responsibilities:

| Persona                | User Type      | Key Needs & Responsibilities                                                                                                 |
| ---------------------- | -------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| **Special Ed Teacher** | Primary User   | Develops and implements IEPs, coordinates services, and monitors student progress. Requires efficient access to comprehensive student information and streamlined documentation tools. |
| **IEP Team Member**    | Secondary User | Includes specialists (e.g., therapists, psychologists) who contribute to assessments and service delivery. Needs collaborative tools and real-time communication. |
| **School Admin**       | Oversight User | Principals and directors who require oversight, reporting functions, and system administration tools for compliance management. |
| **Family Member**      | Stakeholder    | Parents and guardians who need access to their child's information, progress updates, and communication tools to engage with the educational team. |

## 5. User Scenarios & Key Workflows

*   **IEP Development**: The system will guide users through the entire IEP development process, from initial referral to annual reviews, featuring automated compliance checks and deadline management.
*   **Daily Progress Monitoring**: Users can perform streamlined data entry for daily observations, behavioral tracking, and academic progress, with access to visual analytics to identify trends.
*   **Collaborative Document Review**: Multiple users can edit documents in real-time, with features like version control, comments, and approval workflows that maintain a clear audit trail for compliance.

## 6. Feature Requirements

### 6.1. Core Platform Features

| Feature ID | Feature Name                         | Description                                                                                                                                                             | Priority |
| :--------- | :----------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------- |
| CORE-01    | **Student Profile Management**       | Centralized profiles containing personal data (encrypted), educational history, disability classifications, family contacts, and medical information.              | High     |
| CORE-02    | **IEP Document Management**          | Store and manage current and historical IEPs, including goals, service assignments, accommodations, and transition plans.                                               | High     |
| CORE-03    | **Assessment & Progress Data**       | Store and track formal/informal assessment results, progress monitoring data, behavioral data, and related service evaluation reports.                               | High     |
| CORE-04    | **Role-Based Access Control (RBAC)** | Granular user management with permissions based on roles (Admin, Teacher, Specialist, Family) to ensure data privacy and security. Audit trails for all user actions are mandatory. | High     |
| CORE-05    | **File Management System**           | Comprehensive file upload and organization capabilities with support for multiple formats and compliance scanning.                                                     | High     |
| CORE-06    | **Analytics Dashboard**              | Advanced dashboard with visual representations of student progress, goal achievement, service delivery tracking, and compliance status.                                 | High     |

### 6.2. Collaboration Features

| Feature ID | Feature Name                    | Description                                                                                                                                     | Priority |
| :--------- | :------------------------------ | :---------------------------------------------------------------------------------------------------------------------------------------------- | :------- |
| COL-01     | **Collaborative Text Editor**   | A real-time editor for educational documents with concurrent editing, change tracking, comments, and version history.                      | High     |
| COL-02     | **User Presence Indicators**    | Real-time indicators showing which team members are actively viewing or editing a document to prevent conflicting edits.                    | High     |
| COL-03     | **Email Notifications**         | Automated email notifications for important events and updates using the Resend component.                                                    | Medium   |

### 6.3. AI-Powered Features

| Feature ID | Feature Name                | Description                                                                                                                                                                 | Priority |
| :--------- | :-------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :------- |
| AI-01      | **AI-Powered IEP Generation** | Intelligent assistance for creating IEP goals and objectives based on assessment data and student profiles, with human oversight and customization capabilities required. | Medium   |
| AI-02      | **AI Chat Support Agent**   | An integrated intelligent assistant providing immediate support for special education procedures, compliance questions, and system navigation.                          | Medium   |

## 7. Non-Functional Requirements

### 7.1. Compliance & Security
*   **FERPA Compliance**: The system must strictly adhere to the Family Educational Rights and Privacy Act (FERPA) through RBAC, audit logs, and secure communication channels.
*   **IDEA Compliance**: Must include built-in checks for Individuals with Disabilities Education Act (IDEA) requirements, such as timeline management and documentation verification.
*   **Data Encryption**: All personally identifiable information must be encrypted both at rest and in transit.
*   **Security Audits**: The system will undergo regular penetration testing, vulnerability assessments, and privacy compliance audits by third-party professionals.

### 7.2. Accessibility
*   The application must be compliant with **Web Content Accessibility Guidelines (WCAG) 2.1 Level AA**, ensuring it is usable for individuals with disabilities. This includes screen reader compatibility, keyboard navigation, and high contrast modes.

### 7.3. Performance & Reliability
*   **PWA Functionality**: The application must function as a Progressive Web App, with a comprehensive service worker for offline access, a web app manifest for installation, and push notifications for real-time updates.
*   **High Availability**: The system will use a blue-green deployment methodology to minimize downtime during updates. It must have real-time performance monitoring and automated daily backups with point-in-time recovery capabilities.

### 7.4. Technical Stack
*   **Frontend**: Vite/React 18 with TypeScript.
*   **UI Framework**: ShadCn UI.
*   **Backend**: Convex serverless platform.
*   **Authentication**: Better-auth with Convex-auth.
*   **AI Integration**: OpenAI API via Convex actions.
*   **Billing**: Polar integration for subscriptions.
*   **Hosting**: Vercel with edge distribution.

## 8. Out of Scope

*   Integration with non-standard or legacy school information systems not specified in initial requirements.
*   Direct billing to insurance or state medical agencies.
*   Student-facing portals or applications.

## 9. Assumptions and Dependencies

*   Schools will have the necessary infrastructure to support a modern web application.
*   Stakeholders (teachers, administrators, families) are willing to adopt a new digital platform and participate in training.
*   Third-party services (OpenAI, Vercel, Convex, Polar) will maintain stable and reliable APIs and services.