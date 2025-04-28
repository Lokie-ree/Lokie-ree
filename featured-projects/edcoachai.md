# EdCoach AI

EdCoach AI is an instructional support platform for school leaders, instructional coaches, and teachers. The MVP streamlines classroom observations, provides instant, rubric-aligned feedback, and tracks teacher growth at the school level.

## Core MVP Features

- **Role-Based Dashboards:** For teachers, instructional coaches/assistant principals, and principals
- **Observation System:** Two templates (Formal Observation, Informal Walkthrough) using the LER rubric
- **Draft/Finalized Workflow:** Observations can be saved as draft or finalized before sharing
- **AI-Assisted Feedback:** Instantly generate and edit professional feedback based on observation evidence
- **Teacher Feedback Access:** Teachers can view and download observation results and feedback
- **Analytics Dashboard:** Visualize observation trends and teacher performance, scoped to school
- **Authentication:** Secure login and registration with Clerk
- **Role/Permission Management:** Roles and permissions managed in Convex DB for future scalability
- **Responsive Design:** Works on desktop, tablet, and mobile

## Technology Stack

- **Frontend:** Next.js 15, Tailwind CSS, ShadCN UI, MagicUI
- **Backend:** Convex for database and server logic
- **Authentication:** Clerk (Convex DB for roles/permissions)
- **AI:** LLM for educational context and LER rubric alignment

## Development Status

EdCoach AI is in active MVP development, focusing on the core observation-feedback-analytics loop for school-level users.

## Planned Features (Post-MVP)

- Custom rubric support
- District admin features
- Advanced analytics and reporting
- Teacher response to feedback
- Gamification and subscription management

## Getting Started

### Prerequisites

- Node.js
- npm or pnpm
- Clerk account
- Convex account

### Installation

1. Clone this repository
   ```
   git clone https://github.com/yourusername/edcoach-ai.git
   cd edcoach-ai
   ```

2. Install dependencies
   ```
   npm install
   ```

3. Set up environment variables
   - Copy `.env.example` to `.env.local` and fill in required values for Clerk and Convex integration

4. Start the development server
   ```
   npm run dev
   ```

5. Configure Clerk/Convex integration:
   - Open your app. There should be a "Claim your application" button from Clerk in the bottom right of your app.
   - Follow the steps to claim your application and link it to this app.
   - Follow step 3 in the [Convex Clerk onboarding guide](https://docs.convex.dev/auth/clerk#get-started) to create a Convex JWT template.
   - Paste the Issuer URL as `CLERK_JWT_ISSUER_DOMAIN` to your dev deployment environment variable settings on the Convex dashboard (see [docs](https://docs.convex.dev/auth/clerk#configuring-dev-and-prod-instances))

## Learn More

- [Product Requirements Document](documentation/prd.md)
- [Development Roadmap](documentation/development-roadmap.md)
- [Testing Plan](documentation/testing-plan.md)
- [Convex Documentation](https://docs.convex.dev/)
- [Clerk Documentation](https://clerk.dev/docs)

## Contact

For questions or inquiries about EdCoach AI, please reach out to me.