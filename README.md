<!-- BANNER -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:FF6B00,100:0f766e&height=200&section=header&text=Randall%20LaPoint,%20Jr.&fontSize=48&fontColor=ffffff&fontAlignY=38&desc=Interactive%20Learning%20Designer%20%2F%2F%20Full-Stack%20Builder&descSize=18&descAlignY=58" alt="Randall LaPoint, Jr." />
</p>

<!-- ANIMATED TAGLINE -->
<p align="center">
  <a href="https://creative-lab-five.vercel.app/">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=16&duration=3000&pause=800&color=FF6B00&center=true&vCenter=true&width=620&lines=I+build+interactive+experiences+for+hard+ideas;WebGL+%2F%2F+Real-time+full-stack+%2F%2F+RAG+%2F%2F+Agentic+tooling;Everything+ships.+Real+users.+One+deadline." alt="tagline" />
  </a>
</p>

<!-- QUICK LINKS -->
<p align="center">
  <a href="https://creative-lab-five.vercel.app/"><img src="https://img.shields.io/badge/Creative_Lab-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Creative Lab" /></a>
  <a href="http://pelicanai.org"><img src="https://img.shields.io/badge/Pelican_AI-FF6B00?style=for-the-badge&logo=convex&logoColor=white" alt="Pelican AI" /></a>
  <a href="https://www.linkedin.com/in/lapointwebdev/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:rplapointjr@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

---

I'm a mathematician and 15-year educator who now ships **production interactive software, end-to-end** — WebGL/3D learning environments, real-time full-stack apps, RAG-backed AI tooling, and the agentic system that keeps it all coherent. Everything here is **deployed, used by real people every week, and converging on one stage: ISTE LIVE 2026.**

The domain is education. The interesting part is the engineering: rendering 3D geometry that responds to a learner in real time, keeping an LLM grounded in a strict standards corpus, and orchestrating four repos solo against a hard deadline without a monorepo.

---

## 🛠️ Stack

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)

**Frontend & 3D / Motion**

![React](https://img.shields.io/badge/React_19-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Three.js](https://img.shields.io/badge/Three.js-000000?style=flat-square&logo=threedotjs&logoColor=white)
![R3F](https://img.shields.io/badge/React_Three_Fiber-black?style=flat-square&logo=react&logoColor=61DAFB)
![GSAP](https://img.shields.io/badge/GSAP-88CE02?style=flat-square&logo=greensock&logoColor=black)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-0055FF?style=flat-square&logo=framer&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind_v4-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![shadcn/ui](https://img.shields.io/badge/shadcn%2Fui-000000?style=flat-square&logo=shadcnui&logoColor=white)

**Backend & AI**

![Convex](https://img.shields.io/badge/Convex-FF6B00?style=flat-square&logo=convex&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React Router](https://img.shields.io/badge/React_Router_v7-CA4245?style=flat-square&logo=reactrouter&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI_+_RAG-412991?style=flat-square&logo=openai&logoColor=white)
![Better Auth](https://img.shields.io/badge/Better_Auth-000000?style=flat-square&logo=auth0&logoColor=white)

**Tooling**

![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![Storybook](https://img.shields.io/badge/Storybook-FF4785?style=flat-square&logo=storybook&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=flat-square&logo=pnpm&logoColor=white)

---

## 🗺️ System architecture

Two product arcs, one shared brain. **Steel** (an agentic-OS vault) holds canonical facts and keeps the Creative Lab spokes in sync; the educator arc evolved through archived experiments into the live product.

```mermaid
graph TB
    S["⚙️ Steel · Agentic OS Hub<br/>canonical facts · sync registry · sprints"]

    subgraph A1["Arc I · Students — discovery-first math"]
        CL["Creative Lab<br/>R3F · GSAP"]
        I26["ISTE-26<br/>lab guides"]
        CLD["Creative Lab Demos<br/>RR7 · SSR · Docker"]
        PF["Portfolio<br/>R3F · tokens"]
    end

    subgraph A2["Arc II · Educators — AI for the classroom"]
        PA["Pelican AI · LIVE<br/>Convex · RAG · agents"]
        EC["EdCoach AI<br/>archived"]
        SS["SpedSync<br/>PWA · Convex"]
    end

    S --> CL & I26 & CLD & PF
    EC -.->|lessons| PA
    SS -.->|lessons| PA

    style S fill:#1f2937,stroke:#FF6B00,stroke-width:3px,color:#fff
    style PA fill:#0f766e,stroke:#FF6B00,stroke-width:2px,color:#fff
    style CL fill:#0f766e,stroke:#0f766e,color:#fff
    style I26 fill:#0f766e,stroke:#0f766e,color:#fff
    style CLD fill:#0f766e,stroke:#0f766e,color:#fff
    style PF fill:#0f766e,stroke:#0f766e,color:#fff
    style EC fill:#374151,stroke:#6b7280,color:#cbd5e1
    style SS fill:#374151,stroke:#6b7280,color:#cbd5e1
```

---

## 🧪 Arc I — Interactive math, rendered in real time

> The engineering challenge: 3D geometry that responds to a learner mid-gesture, with formulas gated behind demonstrated understanding.

| Project | Engineering highlight | Stack | |
|---|---|---|---|
| **Creative Lab** | Flagship. Earned-reveal module engine; one reusable geometric fixture across the whole Grade 8 arc + Sinewaves + Vector Transformations. | `R3F` `GSAP` `Storybook` | [repo](https://github.com/Lokie-ree/creative-lab) · [live](https://creative-lab-five.vercel.app) |
| **ISTE-26** | Dual-mode guides (teacher config + student log) driven by a shared standards model. | `Vite` `shadcn/ui` | [repo](https://github.com/Lokie-ree/iste-26) · [live](https://iste-26.vercel.app) |
| **Creative Lab Demos** | Server-rendered demo host (Cross-Section Explorer); ships via Docker or Vercel. | `RR7 SSR` `Docker` | [repo](https://github.com/Lokie-ree/creative-lab-demos) · [live](https://creative-lab-demos.vercel.app) |
| **Portfolio** | Live R3F module previews, GSAP scroll choreography, single-source design tokens mirrored to CSS `oklch()` + Three.js hex. | `R3F` `GSAP` | [repo](https://github.com/Lokie-ree/portfolio) · randalllapointjr.dev |

**The reusable fixture:** a single scalene triangle `A(1,1) B(4,2) C(2,4)` is the invariant across every geometry module — the same object transformed three ways (rigid motions → dilations → Pythagorean), so learners deepen one mental model instead of context-switching. It's the same instinct as reusing a well-designed test fixture.

---

## 🤖 Arc II — AI tooling for educators

> The engineering challenge: keep an LLM useful *and* grounded in a strict, real corpus — no hallucinated standards.

| Project | Engineering highlight | Stack | |
|---|---|---|---|
| **Pelican AI** | Live. Prompt coach with RAG over the Louisiana standards + rubric corpus; Convex agents + workflows, auto-save-on-copy, session management. | `Convex` `RAG` `OpenAI` | [repo](https://github.com/Lokie-ree/aida) · [live](http://pelicanai.org) |
| **EdCoach AI** | Archived predecessor. 5-phase growth-loop platform; early experiment in multi-agent dev workflows. | `Next.js` `Convex` | [repo](https://github.com/Lokie-ree/edcoachai) |
| **SpedSync** | Special-education management PWA on a real-time Convex backend. | `Convex` `PWA` | [repo](https://github.com/Lokie-ree/sped-sync) |

EdCoach AI and SpedSync were the experiments. Each returned a lesson — *narrower scope, conversational over dashboard, domain-specific over generic* — that compounded into **Pelican AI**, the one teachers actually use.

---

## ⚙️ Steel — the system behind the system

Coordinating four related repos solo, against a fixed conference date, is a real engineering problem. **[Steel](https://github.com/Lokie-ree/steel)** is the answer: an Obsidian-based agentic-OS hub that every AI session reads first. It holds the canonical facts (module names, coordinates, URLs, standards), a **sync registry** of cross-repo fields, and time-boxed **sprint docs**.

**Drift policy:** freeze structure, document sync points, *no premature monorepo.* When a user-facing string changes, every affected spoke is updated in the same session. Shared packages get reconsidered only after the deadline ships.

---

## 🔬 Validation loop

Built *with* users, not tested *on* them. The **IVLA STEM Club** meets twice weekly and hits every build as learners first — they're also learning the stack that produces it (React, Vite, R3F). The metric is **observable understanding, not survey scores**: it shows up in how they interact, not what they self-report. Continuous, in-the-loop user testing on a weekly cadence.

---

## 📊 GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Lokie-ree&show_icons=true&hide_border=true&theme=tokyonight&title_color=FF6B00&icon_color=FF6B00&include_all_commits=true&count_private=true" alt="GitHub stats" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Lokie-ree&layout=compact&hide_border=true&theme=tokyonight&title_color=FF6B00&langs_count=8" alt="Top languages" />
</p>

---

## 🧭 What's next (post-ISTE)

**Project Studio** — a scoping engine that turns fuzzy student interests into a *finishable* plan. A knowledge-file-backed Gemini Gem runs a six-stage loop (Spark → Expand → Narrow → Shape → Checkpoint → Export); a companion web app generates a scoped plan — goal, out-of-scope boundaries, milestones, and a 48-hour **Milestone Zero** — then hands off to the Gem with a pre-filled prompt. The archetype library compounds into classroom-specific institutional memory.

> The thesis again, one layer up: the hard thing isn't starting a creative project — it's *finishing* one. So I'm engineering "finishable" into the tooling.

---

## 🎓 Background

**Education** — MS Mathematics (Nicholls State) · MEd Educational Leadership (American College of Education) · BS Mathematics (Nicholls State)

**Teaching** — 15 years: algebra, geometry, advanced mathematics, K–6 STEM, mentoring, technology facilitation.

**Now** — building the tools that scale what 15 years in the classroom taught me about how people actually learn.

---

<p align="center">
  <strong>📍 It all converges on ISTE LIVE 2026 · Orlando · June 28 – July 1.</strong>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f766e,100:FF6B00&height=120&section=footer" alt="" />
</p>
