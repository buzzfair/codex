# Presence Pause Product Overview

## 1. Problem Statement
Brian and professionals like him need a compassionate, lightweight way to practice micro-rituals, notice what helps, and reflect on their experiences without the pressure of a traditional productivity tool.

## 2. Solution Summary
Presence Pause is a cross-platform application (Web, iOS, Android) that guides short, values-aligned rituals, makes compassionate permission visible, enables quick logging, schedules gentle reminders, builds a personal playbook of effective practices, and surfaces reflections and patterns without gamification pressure.

## 3. Design Tenets
- Calm, minimal, non-judgmental, values-aligned
- Low friction and privacy-first
- Accessible (WCAG 2.2 AA), offline-friendly experience

## 4. Target Users
### Primary Persona: Brian
- Reflective, introverted professional seeking meaning and reduced self-criticism
- Needs tiny nudges, quick logs, compassionate language, easy reflection, and low effort tools

### Secondary Persona: Coach Guin
- Supports Brian with pattern recognition and micro-experiments
- Requires read-only insights, exportable summaries, and must avoid surveillance feelings

## 5. Core Use Cases & Stories
- **Rituals**: Start in one tap, guided flow (60–120s), optional notes, saboteur naming, anchor selection, gentle scheduling.
- **Connection Ritual**: Human check-in tracking, log colleague details, rolodex of connections.
- **Reflection & Playbook**: Weekly snapshot in <2 minutes, progress without streaks, evolving playbook.
- **Coach View**: Opt-in sharing, revocable access, weekly summary exports, dashboard for coaches.

## 6. MVP Feature Set
### Must-Haves
- Email/password and OAuth authentication (Apple/Google)
- Ritual flows with anchors, saboteur naming, 60s timer
- One-tap logging with optional notes and emotional check-in
- Rule-based reminders with snooze/skip
- Connection ritual logging with details list
- Weekly reflection with prompts and summary view
- Insights (weekly trends, wins feed)
- Export/share weekly summary with revoke
- Offline-first logging, secure syncing
- Accessibility (WCAG AA) and privacy-first onboarding

### Nice-to-Have (v1.1+)
- Calendar integration for auto-blocking micro-resets
- Polished push notifications, voice note logging
- Coach portal with configurable questions

## 7. Information Architecture
Primary tabs: Home (Today), Rituals, Playbook, Insights, Settings.

## 8. Data Model Overview
Entities: Users, Rituals, RitualLogs, WeeklyReflections, ShareLinks. See original specification for schema details.

## 9. State Machines (High Level)
- **Ritual Flow**: IDLE → ACTIVE → REVIEW → LOGGED → IDLE
- **Reminder Flow**: SCHEDULED → TRIGGERED → (Snooze | Start | Skip) → COMPLETE/RESCHEDULED

## 10. UX Flows
- Start reset: Home → Reset → Guided modal → Log feelings/notes → Confirmation
- Connection ritual: Prompt with questions → Log colleague detail → Save
- Weekly reflection: Playbook → 3 prompts → Submit → Summary

## 11. Copywriting Guidelines
Use compassionate, non-judgmental language (e.g., “Every try counts,” “A breath now is a gift to Future You.”) Replace “break” with “Well-being Reset” or “Presence Pause.”

## 12. Accessibility & Inclusion
WCAG 2.2 AA compliance, reduced motion toggle, large hit areas, inclusive language, timezone aware scheduling.

## 13. Privacy & Security
Encryption at rest and in transit, local device encryption, explicit sharing consent, export/delete capabilities, minimal PII, opt-in analytics.

## 14. Tech Stack
- **Frontend**: React + TypeScript (web), React Native + Expo (mobile), Tailwind/NativeWind, React Query, Zustand/Redux Toolkit
- **Backend**: Node.js (NestJS/Express), TypeScript, Postgres + Prisma, Redis, BullMQ/Temporal, JWT auth, Headless Chrome for exports
- **DevOps**: Fly.io/Render/Heroku or AWS, GitHub Actions, CodePush, Sentry/PostHog

## 15. APIs & Integrations
Endpoints for auth, rituals, logs, insights, reflections, share links. Sample payloads for ritual logging provided in the core specification.

## 16. Analytics (Gentle & Privacy-Aware)
Track aggregated ritual counts, anchor usage, reminder responsiveness, reflection completion, with opt-out and no streak pressure.

## 17. Acceptance Criteria
Ensure ability to configure ritual types, complete/log rituals quickly, manage reminders, log connections, complete weekly reflections, export/share summaries, support offline usage, meet accessibility and privacy expectations.

## 18. Visual System
Neutral palette with calming accent, spacious typography (Inter/SF), card-based components, rounded corners, affirming feedback (“Logged. Nicely done.”)

## 19. Roadmap
- **MVP (4–6 weeks)**: Core rituals, logs, reminders, reflections, insights lite, export, offline support.
- **v1.1 (3–4 weeks)**: Calendar blocks, notification polish, coach portal, voice notes.
- **v1.2 (3–4 weeks)**: Pattern insights, relationship helper, richer reflections, theming.

## 20. QA & Testing Plan
Unit tests for scheduling/logging, E2E flows (Playwright/Detox), accessibility audits, offline sync tests, notification verification, load tests for reminders.

## 21. Risks & Mitigations
- Notification fatigue → mindful defaults, easy snooze/disable.
- Privacy concerns → transparent policy, user-controlled sharing.
- Feature creep → protect MVP scope.

## 22. Sample Weekly Summary
- Rituals: Connection 2 • Resets 6 • Regulation 8
- Top anchor: Visual (maple tree)
- Wins: “Closed laptop for 2 min between calls; felt lighter.”
- Blockers: “Forgot on back-to-back days.”
- Next micro-goal: “2 resets/day on Tue & Thu.”
