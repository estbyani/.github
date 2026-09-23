# Estbyani · استبياني

**Ask smarter. Understand faster. Decide with confidence.**

Estbyani (استبياني — Arabic for "my survey") is an AI-powered platform for forms, surveys,
assessments, quizzes, feedback, and data collection. Built Arabic-first and fully multilingual,
it is one place to create surveys, understand the answers, and turn them into decisions with
your team — the *Arabic Engine for More than a Survey*.

🌐 [estbyani.com](https://estbyani.com)  ·  العربية · English · 中文

## What you can do

- **Create with ease** — a fast survey/form builder with autosave, rich question types, theming,
  and conditional logic.
- **Understand faster** — AI reads responses, surfaces patterns and sentiment, and drafts clearer
  questions.
- **Decide with confidence** — turn feedback into a concise, actionable decision brief.
- **Work as a team** — multi-tenant workspaces with roles, invitations, live collaboration, and
  audit trails.
- **Reach everyone** — Arabic (RTL), English, and Simplified Chinese, out of the box.

## Status

Estbyani is being rebuilt with a clearer, faster experience from first question to final insight.
Early access is opening soon — **join the waitlist at [estbyani.com](https://estbyani.com)**.
Existing surveys and responses stay safe, and the free features you rely on remain available.
Estbyani is an independent project.

## Under the hood

A TypeScript + Java monorepo — Turborepo + pnpm for the JS/TS workspace, with an independent
Gradle build for the API:

| Layer | Technology |
|-------|------------|
| Web | Next.js 16 · React · TypeScript · next-intl (RTL-aware) · BFF auth |
| API | Spring Boot 4 modular monolith (Java 25) |
| Data | PostgreSQL · jOOQ · Flyway |
| Identity | Keycloak (authentication) + Estbyani-owned authorization / RBAC |
| Cache & async | Redis |
| Cloud | Oracle Cloud Infrastructure — Object Storage · OKE · Terraform |

**Open specifications** power the product:

- **EFD v1** — the *Estbyani Form Definition*: a canonical, versioned, executable form schema
  (JSON Schemas + shared conformance fixtures) covering question types, logic jumps, recalls,
  matrix/ranking, scored assessments, multilingual content, and theming.
- **Logic Engine** — a specified, safety-checked engine for conditional logic and branching.

Quality is enforced with Vitest, Playwright (end-to-end), and Java integration tests
(Testcontainers).

## Links

- Website & waitlist — [estbyani.com](https://estbyani.com)
- Contact — [info@estbyani.com](mailto:info@estbyani.com)
