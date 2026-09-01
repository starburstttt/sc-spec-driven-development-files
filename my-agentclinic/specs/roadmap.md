# Roadmap

High-level implementation order, broken into very small phases. Each phase
should leave the site in a working, demoable state.

## Phase 1 — Scaffolding

Set up the Next.js + TypeScript project. A single page renders
("Welcome to AgentClinic").

## Phase 2 — Ailments & therapies catalog (static)

Hardcoded list of ailments and their therapies, rendered as simple pages.
No database yet.

## Phase 3 — Booking form (UI only)

A form where an agent picks an ailment/therapy and a time slot. No
backend persistence yet — submission just shows a confirmation.

## Phase 4 — Booking API (in-memory)

Wire the form to a server-side API route that stores bookings in memory.
Submitting the form creates a real booking on the server.

## Phase 5 — Appointment list view

A page listing submitted bookings (still backed by in-memory storage).

## Phase 6 — Persistent storage

Swap in-memory storage for a real database so bookings survive a
restart.

## Phase 7 — Dashboard shell

A dashboard page for agents/staff showing appointments in one place
(Mary's "easy access" ask).

## Phase 8 — Auth

Basic login so the dashboard is only accessible to agents/staff.

## Phase 9 — Visual design pass

Styling and responsiveness pass so the site is attractive and works well
across modern browsers (Steve's ask).

## Phase 10 — Reliability hardening

Error handling, input validation, and general robustness pass before
calling the site reliable (Mary's ask).
