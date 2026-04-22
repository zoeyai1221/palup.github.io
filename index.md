# PalUp
**Finding your next meal companion — one conversation at a time.**

> A mobile app that connects people for shared dining experiences in a new city.

**Role:** UX Researcher & Interaction Designer

**Team:** Siyu (Zoey) Ai, Karena Ma, Suiyang Mai, Xinran Wang

**Timeline:** January – April 2026

**Tools:** Figma, Affinity Diagramming, Semi-structured Interviews

---

## The Problem

Moving to a new city means eating alone — a lot. Communal dishes like hotpot and dim sum lose their appeal without company. Existing platforms like Meetup handle large events, but nothing exists for the simple, recurring need: finding one to three people to share a meal with.

> **Core insight from research:** People don't want a dining companion who likes the same food. They want someone they can actually talk to.

---

## Research

### How we learned what users actually need

We conducted **8 semi-structured interviews** with Chinese immigrants living in Seattle (1–10 years in the US), recruited from our personal networks. Sessions were split between in-person and Zoom. Participants ranged in age and gender, and were selected for living alone or having limited social networks in the city.

**[PLACEHOLDER: Affinity Diagram photo/screenshot]**
*Caption: Affinity diagram clustering 6 major themes from interview data*

Key themes that emerged:

- **Conversation > cuisine** — participants consistently prioritized conversational fit over food preferences when evaluating potential dining companions
- **Group size matters** — 4 people was cited as ideal: small enough to talk meaningfully, large enough to reduce awkward silences
- **Safety is a prerequisite, not a bonus** — especially for female participants, trust mechanisms were non-negotiable
- **The bad cycle** — fewer friends → less dining out → harder to meet people

---

## User Persona

**[PLACEHOLDER: Angela Zhang persona image]**

*Angela, 28 — Software Engineer, Seattle. Loves communal dining, struggles to find compatible companions without it feeling like a date.*

---

## Design Process

Four iterative phases, each building on what we learned.

**[PLACEHOLDER: Process timeline diagram — Research → Sketch → Wireframe → Prototype]**

---

### Phase 1 — Paper Prototype

We sketched four core task flows: managing a profile, finding and joining an event, creating an event, and chatting with participants. Each team member owned one flow.

**[PLACEHOLDER: Paper prototype photo — Create Event flow]**
**[PLACEHOLDER: Paper prototype photo — Chatroom / View Events flow]**
**[PLACEHOLDER: Paper prototype photo - before eval]**
**[PLACEHOLDER: Paper prototype photo - after eval]**

A cross-team heuristic evaluation surfaced 12 issues. The most severe:
- No send button visible in the chat interface
- No way to leave a chatroom
- Event creation and home browsing shared the same screen; users didn't know which mode they were in

---

### Phase 2 — Wireframes (Low-Fidelity)

We moved into Figma and connected all flows into an interactive prototype. Major fixes from heuristic evaluation:

- Added a floating "+" button as a dedicated event creation trigger
- Added error states to the login flow
- Separated browsing and creating into distinct screens

**[PLACEHOLDER: Figma wireframe screenshot — Home + Create Event screens]**
**[PLACEHOLDER: Figma wireframe screenshot — Chatroom screen]**
**[PLACEHOLDER: Figma wireframe screenshot — Login error screen]**

---

### Phase 3 — Medium-Fidelity Prototype

User testing with 4–5 participants revealed two persistent issues in the Create Event flow:

- Newly posted events on the Home screen weren't tappable; users had to navigate to My Events
- The "Vibe" field label (options: Quiet / Casual / Deep) confused participants who couldn't interpret what it meant

**Changes made:**
- All event cards made tappable across every screen
- "Vibe" renamed to **Dining Atmosphere** with options: Quiet Meal / Casual Hangout / Deep Conversation

**[PLACEHOLDER: Medium-fi prototype screenshot — Create Event preferences screen]**
**[PLACEHOLDER: Medium-fi prototype screenshot — Event detail page with tappable card]**

---

### Phase 4 — High-Fidelity Prototype

A second round of user testing and expert critique pushed the design further. Key changes:

| Issue Found | Fix Applied |
|---|---|
| "Budget" vs. total cost ambiguity | Renamed to **Budget/Person** |
| Group size unclear if creator counted | Added hint: *incl. yourself* |
| Cancel/Edit only accessible from My Events | Added buttons directly on event detail page |
| Chat input field below keyboard | Repositioned above keyboard (standard mobile pattern) |
| Mute toggle had no visible feedback | Replaced with **pinned notice** at top of chatroom |
| Report reason locked after selection | Made reason editable before submission |

**[PLACEHOLDER: HF prototype screenshot — Home screen]**
**[PLACEHOLDER: HF prototype screenshot — Create Event flow]**
**[PLACEHOLDER: HF prototype screenshot — My Event page]**
**[PLACEHOLDER: HF prototype screenshot — Chatroom with pinned notice]**
**[PLACEHOLDER: HF prototype screenshot — Profile page]**

🔗 [View the full interactive prototype →](https://www.figma.com/proto/GHEjNtXC88rwqjANMyj82r/PalUp?node-id=628-2444&t=9MffpE68rPn1Mh8K-1)

---

## Evaluation

### What we tested and what we found

We conducted in-person user testing across two rounds (heuristic evaluation + think-aloud sessions), with 4–5 participants each. All participants were new to the prototype. There was no prior exposure to the design.

**Four task flows were evaluated:**

1. Log in and manage profile
2. Find and join a dining event
3. Create a dining event
4. Communicate in a chatroom

**Notable findings:**

- Field label clarity was the most recurring friction point across tasks — small wording changes (Budget/Person, Dining Atmosphere) had outsized impact on user confidence
- Navigation consistency mattered: users expected the same action to be available regardless of which screen they entered from
- The chatroom pinned notice was well-received — participants said it reduced the need to scroll up for key event details
- Safety-related features (report flow, profile previews) were expected by participants even when not prompted

**[PLACEHOLDER: Usability issues table screenshot or graphic]**

---

## Reflection

**What worked:** Grounding design decisions in a specific, counterintuitive research finding, like conversational fit matters more than food preference, gave the team a clear north star throughout iterations. Every field label and feature choice could be evaluated against that principle.

**What we'd do differently:** Our participant pool skewed toward Chinese international students, limiting the generalizability of findings. A more diverse sample would have surfaced different safety concerns, dining norms, and social dynamics. We also would have introduced quantitative usability metrics (SUS, task completion rates) earlier in testing.

**What's next:** A matching algorithm surfacing compatible companions, verified profiles to address safety concerns, and an empty-state experience for newly created events with no joiners yet.
