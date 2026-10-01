# SERP — Smart Emergency Response Platform

> AI-assisted, human-in-the-loop decision support for emergency dispatch.

SERP is a web-based decision-support platform designed to assist emergency dispatchers in managing incidents more efficiently. It uses AI to recommend incident priority and suitable emergency units based on incident information — while the final decision always remains with the human dispatcher.

> **Status:** 🚧 **Under active development / in progress.** SERP is my university graduation project at the German Jordanian University (GJU). This case study showcases what has been designed and implemented so far, alongside capabilities that are planned or in development. It is **not** a finished production system.

---

## Role & Context

- **Role:** Sole developer — responsible for the full project lifecycle, including system design, backend development, frontend development, AI-assisted decision-support features, and integration.
- **Type:** University graduation project at the German Jordanian University (GJU), developed solo.
- **Timeframe:** 2026 academic project period (ongoing).

---

## Problem

Emergency dispatchers have to make time-sensitive decisions based on incoming incident information — determining how urgent an incident is and which available units should respond.

When information is incomplete, or when multiple incidents compete for attention, these decisions become more challenging and time-consuming. SERP was designed to support the dispatcher by providing consistent, AI-assisted recommendations for incident priority and unit assignment, while keeping the human dispatcher responsible for the final decision.

---

## Solution

SERP is a web-based **dispatch cockpit** that brings several integrated components together around the dispatcher's workflow. Each item below is marked with its current status.

- **Incident Management** — Create, view, and manage emergency incidents and their relevant information. _(Implemented)_
- **AI Priority Recommendation** — Analyzes incident information and recommends an appropriate priority level to support faster triage. _(Implemented)_
- **AI Dispatch Recommendation** — Recommends suitable available emergency units for an incident based on the available information. _(Implemented)_
- **Emergency Call Recording** — Incoming emergency calls can be automatically recorded and associated with the corresponding incident, preserving the conversation as part of the incident record. _(Planned / in development)_
- **Live Map** — A map-based interface giving a visual view of incidents and emergency units. _(Implemented)_
- **Unit Simulation** — Simulated emergency units can change status and location to create a controlled dispatch environment without connecting to real emergency-service systems. _(Implemented)_
- **Decision Audit Trail** — Records key dispatcher decisions and AI recommendations to make the decision-making process traceable. _(Implemented)_
- **Authentication & Roles** — Different user roles can access the system according to their responsibilities. _(Implemented)_
- **Administration** — Administrative functionality allows authorized users to manage the system. _(Implemented)_

The central idea is to combine these components in one dispatcher cockpit, where **AI provides recommendations but the human dispatcher remains in control of the final decision.**

---

## Spotlight: Emergency Call Recording _(Planned / In Development)_

A capability being designed into SERP to strengthen the incident record and support the dispatcher during live response:

1. **Call intake** — An emergency call comes into the dispatch workflow.
2. **Automatic recording** — The call is automatically recorded.
3. **Incident association** — The recording is linked to the corresponding incident.
4. **Preserved record** — The conversation is preserved as part of the incident record, supporting traceability and the dispatcher's response workflow.

> This feature is described as a **planned / in-development** capability. The exact implementation is still being finalized, and it is not presented as fully implemented.

---

## Key Highlights

1. **Human-in-the-loop AI** — AI provides priority and dispatch recommendations, but the dispatcher always makes the final decision. The system is designed to support human judgment rather than replace it.
2. **AI-assisted dispatch decisions** — SERP goes beyond simply displaying incidents by actively helping the dispatcher prioritize incidents and identify suitable available units.
3. **Emergency call recording** _(in development)_ — Automatic recording of emergency calls and association with the relevant incident, preserving the conversation as part of the case record.
4. **Decision audit trail** — AI recommendations and dispatcher decisions are recorded, making the decision-making process traceable and reviewable.
5. **Emergency-unit simulation** — Simulated emergency units, statuses, locations, and incident activity create a controlled dispatch environment without relying on real emergency-service infrastructure.
6. **Integrated dispatch cockpit** — Incident management, AI recommendations, call handling, mapping, unit simulation, and administration are brought together in one interface designed around the dispatcher's workflow.

---

## Tech Stack

| Area | Technologies |
|------|--------------|
| **Frontend** | React, TypeScript, HTML/CSS |
| **Backend** | C#, ASP.NET Core Web API, .NET 9 |
| **Database** | _To be confirmed_ |
| **AI / ML** | AI-assisted recommendation logic for incident priority and emergency-unit assignment _(exact model/approach to be specified)_ |
| **Mapping** | _To be confirmed_ |
| **Hosting / Deployment** | _To be confirmed_ |
| **Tooling** | Git/GitHub, Visual Studio |

---

## Challenges & How I Solved Them

**1. Designing AI recommendations while keeping the dispatcher in control**
I needed to make the AI useful without treating its recommendation as an automatic decision. I designed the workflow so the system presents recommendations clearly, while the dispatcher remains responsible for reviewing and approving the final action.

**2. Creating a realistic emergency-unit simulation**
Because SERP is an academic project and is not connected to real emergency-service infrastructure, I needed to simulate unit availability, status, and movement in a way that makes the dispatch workflow feel realistic. I designed the simulation layer around changing unit states and locations so the dispatcher can interact with a dynamic environment.

**3. Building an integrated system as a solo developer**
The project combines incident management, AI-assisted recommendations, mapping, unit simulation, authentication, administration, and auditability. I kept the architecture modular and separated responsibilities across the system so the project remained manageable and maintainable.

---

## Results & Current Progress

SERP is an **in-progress graduation project**, and its value is measured by what it demonstrates as an end-to-end emergency dispatch decision-support platform.

So far, the project brings together incident management, AI-assisted priority and dispatch recommendations, emergency-unit simulation, mapping, authentication and roles, and a decision audit trail in one dispatcher-focused interface. Additional AI-assisted capabilities — including emergency call recording — are planned or in development.

I tested the main workflows and system components to verify that the core dispatch workflow functions as intended, including incident management, AI recommendations, simulated units, and decision recording.

Since SERP is an academic graduation project still under development — not a production emergency-services system — I make **no claim of real-world operational impact, real emergency-service usage, or deployment**. The value is in demonstrating how AI-assisted decision support could be integrated into an emergency dispatch workflow while keeping the human dispatcher in control.

**Future / planned work:** completing the AI emergency call recording capability, confirming remaining technical choices, evaluating the recommendation logic with larger and more realistic datasets, improving the simulation, and eventually validating the concept with real emergency-service workflows and domain experts.

---

## Screenshots & Visuals

_Approved screenshots, UI visuals, and diagrams will be added here._

---

## Links

- **Demo video:** _Coming soon_
- **Project presentation / documentation:** _Coming soon_
- **LinkedIn:** _To be added_

---

> **Note:** This repository is a portfolio case study for a graduation project that is currently **under development**. It intentionally contains **no source code** and exposes no private, company, or project-internal files.
