### **Product Requirements Document: LEAP Forward**

| **Document Status:** | **Final** |
| :--- | :--- |
| **Version:** | **1.1** |
| **Author:** | AI Agent (In consultation with Project Lead) |
| **Date:** | July 11, 2025 |

### 1. Introduction

#### 1.1. Problem Statement

School districts struggle to provide consistent, high-quality instructional support at scale. Human instructional coaches are a limited resource, and teachers often lack the time and tools to effectively translate dense educational frameworks (like state rubrics and standards) into daily classroom practice. There is a critical need for a tool that can amplify the impact of expert coaches and make instructional excellence accessible to every teacher, every day.

#### 1.2. Vision

To empower every Louisiana teacher with an AI-powered partner that demystifies instructional excellence, seamlessly integrating the Louisiana Educator Rubric (LER), NIET standards, and local LEADs initiatives into their daily planning, reflection, and growth.

### 2. Goals and Objectives

*   **Primary Goal:** To improve teacher effectiveness and student outcomes by providing scalable, personalized, and standards-aligned instructional support.
*   **Objective 1:** Reduce the time teachers spend on lesson planning and resource creation by automating the generation of standards-aligned materials.
*   **Objective 2:** Increase teachers' understanding and application of the LER and NIET frameworks in their daily practice.
*   **Objective 3:** Amplify the reach and impact of instructional coaches by scaling their expertise through an AI partner.
*   **Objective 4:** Provide educational leaders with actionable, data-driven insights into the professional development needs of their staff.

### 3. User Personas

*   **Teacher (Primary User):**
    *   **Goals:** Wants to create high-quality, engaging lessons that meet state standards; wants to save time; needs clear, practical guidance on how to improve their craft.
    *   **Pain Points:** Limited planning time; finds rubric and standard documents dense and hard to apply; feels isolated and lacks on-demand support.
*   **Instructional Coach (Secondary User):**
    *   **Goals:** Wants to support as many teachers as possible; needs to identify systemic instructional challenges; wants to share best practices effectively.
    *   **Pain Points:** Limited bandwidth; cannot be in every classroom at once; struggles to scale their expertise.
*   **Administrator / District Leader (Tertiary User):**
    *   **Goals:** Wants to ensure a return on investment for software; needs to manage user access and billing for the district; desires high-level data on instructional trends.
    *   **Pain Points:** Managing multiple software subscriptions; justifying costs; making data-informed decisions about professional development spending.

### 4. Feature Requirements

#### 4.1. Core System & Authentication
*   **4.1.1.** The system shall provide a secure user authentication system (sign-up, sign-in, password reset).
*   **4.1.2.** Users shall be assigned one of three roles: Teacher, Coach, or Admin.
*   **4.1.3.** Access to features shall be restricted based on the user's assigned role.
*   **4.1.4.** The system must support multi-tenancy, isolating all data (users, documents, chats) by the user's school district.

#### 4.2. Document Management
*   **4.2.1.** Teachers must be able to upload curriculum documents in `.pdf` and `.docx` formats.
*   **4.2.2.** The user interface shall display a list of all documents uploaded by the user.
*   **4.2.3.** The UI must show the processing status of a newly uploaded document (e.g., "Processing," "Ready").
*   **4.2.4.** Teachers must be able to select a specific document to serve as the primary context for an AI chat session.
*   **4.2.5.** Teachers must be able to delete their own documents.
*   **4.2.6.** The system shall provide an option to export AI-generated content (e.g., lesson plans) to common formats like `.docx` and `.pdf` for easy integration into existing workflows.

#### 4.3. AI Chat Interface
*   **4.3.1.** The system shall provide a real-time chat interface for users to interact with the AI partner.
*   **4.3.2.** The chat history for a given session must be saved and displayed.
*   **4.3.3.** The AI's responses must be primarily informed by the content of the user-selected curriculum document and the foundational knowledge base.
*   **4.3.4.** The AI must adopt a supportive, knowledgeable "Coach Persona" in its responses.

#### 4.4. Actionable Generation
*   **4.4.1.** The UI shall provide clear "action buttons" or commands that allow users to generate specific types of content.
*   **4.4.2.** The system shall be able to generate lesson plan outlines based on the active curriculum context.
*   **4.4.3.** The system shall be able to generate formative assessments (e.g., exit tickets, bell ringers) aligned with the active context.
*   **4.4.4.** All generated content must be aligned with the principles of the LER and NIET frameworks.
*   **4.4.5.** A mechanism shall be in place to allow for quality assurance of AI-generated content, potentially through user feedback or coach review flags.

#### 4.5. Coach's Knowledge Base
*   **4.5.1.** Users with the "Coach" role must have access to a separate interface to contribute to a curated knowledge base.
*   **4.5.2.** These "Coach's Notes" will be treated as a prioritized source of truth by the AI, influencing its guidance and suggestions.

#### 4.6. Analytics Dashboard
*   **4.6.1.** Users with "Coach" or "Admin" roles must have access to a private, anonymized analytics dashboard.
*   **4.6.2.** The dashboard must visualize aggregated data, such as the most frequently discussed LER/NIET indicators across the district.
*   **4.6.3.** The dashboard must not display any personally identifiable information or individual chat content.

#### 4.7. User Onboarding
*   **4.7.1.** Upon first login, users shall be presented with a brief, guided tutorial highlighting the core features of the application.
*   **4.7.2.** The system will be pre-populated with sample documents and example chat sessions to demonstrate effective usage patterns.

### 5. The Knowledge Base
The AI's intelligence is a composite of four distinct sources, which must be queryable and used as context for generating responses.
1.  **Foundational Frameworks:** The full text of the Louisiana Educator Rubric (LER) and NIET instructional standards, serving as the base layer of pedagogical truth.
2.  **District Initiatives:** District-specific documents, such as LEADS or Professional Growth Plan (PGP) guidelines, uploaded by an Admin.
3.  **Curriculum Resources:** The specific `.pdf` or `.docx` files uploaded by an individual teacher.
4.  **Curated Expertise:** The high-priority "Coach's Notes" added by instructional coaches.

### 6. Business & Monetization Requirements
*   **6.1.** The product will be sold as a Business-to-Business (B2B) Software as a Service (SaaS).
*   **6.2.** The pricing model will be a recurring subscription, sold to school districts, likely on a per-teacher, per-year basis.
*   **6.3.** The system must integrate with **Polar** to handle all subscription management, checkout flows, and payment processing.
*   **6.4.** Admins must have access to a customer portal (provided by Polar) to manage their district's subscription.
*   **6.5.** Access to the application's features will be gated by the district's subscription status.

### 7. Technical, Performance & Security Requirements
#### 7.1. Technical Stack
The following technologies have been pre-selected and must be used for development:
*   **Frontend:** Vite, React, `react-router-dom`
*   **Styling:** Tailwind CSS, `shadcn/ui`
*   **Backend & Database:** Convex
*   **Authentication:** `better-auth` for Convex
*   **Core AI Logic:** Retrieval-Augmented Generation (RAG) using the `@convex-dev/agent` and `@convex-dev/rag` components.

#### 7.2. Performance Specifications
*   **7.2.1. AI Response Time:** P95 (95th percentile) for AI-generated text responses must be under 10 seconds.
*   **7.2.2. Document Processing:** A standard 10-page document must be processed and ready for chat within 60 seconds of upload.
*   **7.2.3. System Availability:** The service must maintain a 99.5% uptime.
*   **7.2.4. Scalability:** The system must be architected to support up to 1,000 concurrent users per district.

#### 7.3. Security & Compliance
*   **7.3.1. FERPA Compliance:** The application will be designed in accordance with the Family Educational Rights and Privacy Act (FERPA). No personally identifiable student information will be stored or requested.
*   **7.3.2. Data Privacy:** All user data will be encrypted both in transit (TLS 1.2+) and at rest.
*   **7.3.3. Data Retention:** A clear data retention policy will be defined. Upon subscription termination, district data will be retained for 90 days before permanent deletion.

### 8. Success Metrics
*   **Engagement:** Daily Active Users (DAU), average session length, feature adoption rate for "Actionable Generation."
*   **Value:** Number of AI-generated resources created and exported.
*   **Quality:** User ratings or flags on the quality of AI-generated content.
*   **Business:** District subscription renewal rate, conversion rate from trial to paid.

### 9. Out of Scope for Version 1.0
*   Direct, real-time integration with third-party Learning Management Systems (LMS) or cloud storage (e.g., Google Drive).
*   Real-time collaboration features between users (e.g., shared chat sessions).
*   Native mobile applications (iOS/Android).

---