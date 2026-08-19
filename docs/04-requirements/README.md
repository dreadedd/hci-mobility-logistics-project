# Requirements Definition

## Purpose

This document translates the findings from user research — the [Campus Mobility Survey (n=35)](../03-research-analysis/Survey_Analysis.md) — into concrete user needs and design requirements for the mobility and logistics interface. It is the input to Wireframing (stage 5) and High-Fidelity Design (stage 6).

## Source Evidence

- [Survey_Analysis.md](../03-research-analysis/Survey_Analysis.md) — analysis of 35 Google Form responses from University of Ghana students
- [Survey_Responses.csv](../02-user-research/evidence/Survey_Responses.csv) — raw survey data
- Interview photos exist in `docs/02-user-research/interviews/` as process evidence, but no transcript/notes are available yet — interview findings are **not** reflected below and should be added once notes exist.

## User Needs

Derived directly from the survey's top problems and top feature requests:

| # | User Need | Evidence |
|---|---|---|
| UN1 | As a student, I need to find buildings and lecture halls quickly so I am not late or lost on a large campus. | Top problem (14/35); top open-text complaint about confusing/abbreviated building names |
| UN2 | As a student, I need to know where and when a shuttle/bus will arrive so I don't waste time waiting blindly. | 2nd/3rd most common problems (12/35, 11/35); "live shuttle locations" is the #2 most-wanted feature (21/35) |
| UN3 | As a student, I need clearly marked pickup points so I know where to wait for transport. | Unclear pickup points (8/35); Pickup-point locations wanted by 12/35 |
| UN4 | As a student, I need to see transport costs upfront so I can plan and compare options. | Dominant open-text frustration theme (~10 mentions); Transport fares wanted by 12/35 |
| UN5 | As a student, I need a single map that shows the whole campus interactively rather than relying on generic maps or asking people. | #1 most-wanted feature (23/35); 13/35 currently rely on asking another person to navigate |
| UN6 | As a student, I want to be notified about delays or service disruptions so I can adjust my plans. | Requested by 8/35 |
| UN7 | As a student with accessibility needs, I want accessibility information about routes and transport. | Requested by 9/35 |

## Functional Requirements

| ID | Requirement | Priority (MoSCoW) | Related User Need |
|---|---|---|---|
| FR1 | The system shall display an interactive campus map showing buildings, lecture halls, and points of interest. | Must | UN1, UN5 |
| FR2 | The system shall provide search and turn-by-turn directions to any building or lecture hall on the map. | Must | UN1, UN5 |
| FR3 | The system shall display live locations of campus shuttles/buses on the map. | Must | UN2 |
| FR4 | The system shall show estimated arrival times for shuttles/buses at a given stop. | Must | UN2 |
| FR5 | The system shall display and clearly label designated pickup points for shuttles, taxis, and ride-hailing. | Must | UN3 |
| FR6 | The system shall display shuttle/bus route information (which routes serve which stops). | Should | UN2 |
| FR7 | The system shall display estimated or reference transport fares (taxi/ride-hailing) alongside route/trip information. | Should | UN4 |
| FR8 | The system shall send notifications for delays or service disruptions affecting a user's saved or nearby routes. | Should | UN6 |
| FR9 | The system shall surface accessibility information (e.g. step-free routes, ramps) for buildings and routes. | Could | UN7 |
| FR10 | The system shall allow a user to report an issue (e.g. inaccurate pickup point, broken signage) from the map. | Could | UN1, UN3 |

## Non-Functional Requirements

| ID | Requirement | Rationale |
|---|---|---|
| NFR1 | The map and directions must load and be usable on low/mid-range Android devices and slower campus wifi/mobile data. | Target users are students; several open-text responses mentioned campus wifi/connectivity issues |
| NFR2 | Core navigation tasks (find a building, check shuttle arrival) must be completable within a few taps, without account creation, to minimise friction for first-time/occasional users. | 89% of respondents move around campus multiple times a day — the tool must support quick, repeated use |
| NFR3 | The interface must remain legible outdoors in direct sunlight (high-contrast mode). | Primary use context is outdoor, on-campus, walking |
| NFR4 | Location data (live shuttle tracking) should update frequently enough to be trustworthy (target: near real-time) without excessive battery drain. | "Live shuttle locations" was the #2 most-requested feature — trust depends on accuracy |
| NFR5 | The interface should follow accessibility best practices (text scaling, colour contrast, screen-reader support) as a baseline, independent of FR9. | General usability/accessibility principle for a student population that includes users with accessibility needs |

## Out of Scope (for now)

- Payment processing for fares/tickets — research indicates cost is a major frustration, but no evidence yet that in-app payment is expected/requested; revisit after requirements are validated with interviews.
- Booking/reserving a specific ride-hailing trip — only 4/35 use ride-hailing apps regularly; integrating with Bolt/Uber/Yango APIs is a larger undertaking not yet justified by evidence.
- Indoor/room-level navigation within buildings — no direct evidence requested this; "finding lecture halls" refers to locating buildings, not rooms within them.

## Open Items Requiring Further Research

- Interview data is not yet available to validate/deepen these requirements — revisit this document once interview notes exist.
- Confirm which specific shuttle routes/stops exist on campus (needed to scope FR3–FR6 concretely).
- Confirm whether "transport fares" (FR7) should cover only campus shuttle or also third-party taxi/ride-hailing estimates.
- Sample was 80% Level 200 students — consider a small follow-up pass with Level 100/300/400 and postgraduate students, and with staff/drivers, before finalising requirements.

## Traceability Summary

Every "Must" requirement (FR1–FR5) maps directly to one of the two dominant problem clusters identified in the survey analysis: **wayfinding to buildings/lecture halls** and **shuttle/transport unpredictability**. "Should" and "Could" requirements address secondary but still notable needs (cost transparency, delay notifications, accessibility). This keeps the initial wireframing scope tightly grounded in evidence rather than assumption.
