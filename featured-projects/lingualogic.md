# LinguaLogic - K-5 English Language Learning Platform

LinguaLogic is an interactive learning platform designed specifically for K-5 English Language Learners (ELLs). The platform focuses on building foundational English language structure through engaging, Science of Reading (LETRS)-aligned modules.

The product emphasizes interactive exploration over rote memorization, with a visually intuitive interface designed for young learners. LinguaLogic prioritizes privacy-first design principles, ensuring compliance with COPPA regulations while delivering effective educational content.

This project is built using the Convex + Next.js + Clerk template.

## Core MVP Features

*   **User Authentication:** Secure, age-appropriate sign-in using Clerk, ensuring COPPA compliance.
*   **Interactive Learning Modules:** Visually engaging, manipulative activities focused on foundational concepts (phonemic awareness, phonics, morphology, syntax) aligned with the Science of Reading (LETRS).
*   **Learning Path Navigation:** Sequential progression through concepts with visual indicators of completed and available modules.
*   **User Dashboard:** Visual overview of student progress, recent activity, and recommended next steps.
*   **Cross-device Compatibility:** Responsive design optimized for tablets and desktops.

## Future Considerations / Non-Goals (MVP)

*   Comprehensive English curriculum covering all language domains.
*   Advanced 3D interactions.
*   Admin tools for teachers.
*   Content for learners beyond grade 5.
*   Direct replacement for teacher instruction.
*   Learning Management System (LMS) integrations.

## Technology Stack

*   **Frontend:** Next.js 15+, React 19+
*   **Backend/DB:** Convex 1.x+
*   **Deployment:** Vercel
*   **UI:** ShadCn/ui, Tailwind CSS 4+
*   **Auth:** Clerk (@clerk/nextjs 6.x+)
*   **Animation:** Framer Motion
*   **Icons:** Lucide React
*   **Language:** TypeScript 5.x+

## Get started (Initial Setup)

This assumes you are starting from the `create-convex` template for Next.js + Clerk.

If you just cloned this codebase and didn't use `npm create convex`, run:

```bash
npm install
npm run dev
```

If you're reading this README on GitHub and want to use this template, run:

```bash
npm create convex@latest -- -t nextjs-clerk
```

Then follow the setup steps:

1.  Open your app. There should be a "Claim your application" button from Clerk in the bottom right of your app.
2.  Follow the steps to claim your application and link it to this app.
3.  Follow step 3 in the [Convex Clerk onboarding guide](https://docs.convex.dev/auth/clerk#get-started) to create a Convex JWT template.
4.  Uncomment the Clerk provider in `convex/auth.config.ts`
5.  Paste the Issuer URL as `CLERK_JWT_ISSUER_DOMAIN` to your dev deployment environment variable settings on the Convex dashboard (see [docs](https://docs.convex.dev/auth/clerk#configuring-dev-and-prod-instances))

If you want to sync Clerk user data via webhooks, check out this [example repo](https://github.com/thomasballinger/convex-clerk-users-table/).

## Learn more (Convex Resources)

To learn more about developing your project with Convex, check out:

*   The [Tour of Convex](https://docs.convex.dev/get-started) for a thorough introduction to Convex principles.
*   The rest of [Convex docs](https://docs.convex.dev/) to learn about all Convex features.
*   [Stack](https://stack.convex.dev/) for in-depth articles on advanced topics.

## Join the community

Join thousands of developers building full-stack apps with Convex:

*   Join the [Convex Discord community](https://convex.dev/community) to get help in real-time.
*   Follow [Convex on GitHub](https://github.com/get-convex/), star and contribute to the open-source implementation of Convex.