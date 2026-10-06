# 04 - Benchmark Findings & Design Decisions

> **Benchmark Phase:** Phase 2 — Competitive Reference
> **Analysis Date:** October 2026
> **Layer (Garrett):** Scope (feature decisions) & Strategy (positioning)
> **Inputs:** Tool 01 (Civitas Learning), Tool 02 (EAB Navigate360), Tool 03 (Salesforce Education Cloud)

This document synthesizes the strategic opportunities identified across the three benchmarked tools and details the explicit architectural bridge to our **Low-Fi wireframes** and **navigation flows**.

---

## 1. Key Strategic Opportunities & Unmet Market Gaps

1. **Shift from "Risk Cataloging" to "Empathetic Contact Suggestions" (Inspired by Civitas & EAB):**
   * *Gap:* Direct retention tools focus on categorizing students into public "At-Risk Lists" (see Tool 01, Section 3; Tool 02, Section 3).
   * *Opportunity:* PLANAG / PLANAC surfaces a private feed of "Contact Suggestions" to Directors. While Civitas uses Generative AI to suggest tone (Tool 01, Section 5.2), our system integrates predefined empathetic templates that allow students to select their preferred meeting time.

2. **Transparent Expression of Algorithmic Uncertainty:**
   * *Gap:* Existing tools present rigid percentage scores or binary flags (Tool 01, Section 5.1; Tool 02, Section 5.1).
   * *Opportunity:* We eliminate hard percentages and traffic-light colors. Instead, we express confidence levels in plain language (e.g., *"3-week attendance trend"*, *"based on incomplete LMS data"*).

3. **Confidential Closed-Loop Referrals & Discreet Help Channel (Inspired by Starfish & Mobile References):**
   * *Gap:* Standard institutional platforms do not provide a discreet channel for students to request support without feeling judged or exposed to peers (Tool 02, Section 5.3).
   * *Opportunity:* Adopting Starfish's closed-loop model (Tool 02, Section 5.3), students can quietly request peer tutoring or accept director check-ins directly on their mobile devices, keeping conversation details strictly private between assigned roles.

---

## 2. Navigation & UI Pattern Adoption / Rejection

To construct our **Low-Fi Wireframes** and **Information Architecture**, we explicitly adopt or reject established domain patterns:

| Evaluated UX Pattern | Origin Tool | Decision | Justification |
| :--- | :--- | :--- | :--- |
| **Traffic Light Badges (Red/Yellow/Green)** | Tool 01 – Civitas Learning | **⭐ REJECTED** | Produces student anxiety, stigma, and classroom bias (Tool 01, Section 6). Replaced with neutral contextual text badges. |
| **Automated Penalty / Warning Emails** | Tool 01 – Civitas Learning | **⭐ REJECTED** | Punitive automated notices lead to student isolation. Replaced with Director-managed empathetic contact templates. |
| **Generative Tone Assistance** | Tool 01 – Civitas Learning | **ADOPTED (MODIFIED)** | Predefined empathetic templates that eliminate accusatory tones and focus on offering support. |
| **Closed-Loop Case Status** | Tool 02 – EAB Navigate360 | **ADOPTED** | Allows Directors to know that contact or tutoring occurred without accessing private conversation details. |
| **Mobile Card Feed & Bottom Navigation** | Tool 02 – EAB Navigate360 | **ADOPTED** | Aligns with local student habits for low-friction self-tracking and discrete help requests. |
| **Gamified Leaderboards (Kudos, Streaks)** | Tool 02 – EAB Navigate360 | **⭐ REJECTED** | Public leaderboards generate peer pressure and academic stigma — contradicts our non-punitive principle. |
| **Enterprise Case Management (Student 360)** | Tool 03 – Salesforce Education Cloud | **REJECTED** | Overkill for a single-institution tool; adds unnecessary complexity to the student flow. |

⭐ = Dimensions where PLANAG / PLANAC differentiates positively.

---

## 3. Features Explicitly Out of Scope

| Feature | Origin Tool | Why Excluded |
| :--- | :--- | :--- |
| Multi-semester Degree Planner | Tool 01 – Civitas Learning | Out of project scope; we focus on early contact, not curriculum planning. |
| Gamified Kudos / Leaderboards | Tool 02 – EAB Navigate360 | Generates peer pressure and stigma — contradicts our non-punitive design principle. |
| Enterprise Case Management | Tool 03 – Salesforce Education Cloud | Overkill for a single-institution, lightweight tool. |
| Multi-Departmental Communication Logs | Tool 03 – Salesforce Education Cloud | Conflicts with our privacy-by-design principle; students should not be visible across departments. |

---

## 4. Bridge to Low-Fi Wireframes & Navigation Flow

The adopted patterns directly inform the following Low-Fi decisions:

* **Bottom Navigation Bar** (from Tool 02) → used as the primary navigation for the student mobile view.
* **Card Feed with Contact Suggestions** (from Tool 01, modified) → used as the Director's home screen.
* **Closed-Loop Status Indicators** (from Tool 02) → used to notify referring Directors when a case is closed, without exposing private details.
* **Neutral Contextual Text Badges** (replacing Tool 01's traffic lights) → used to convey algorithmic uncertainty.
* **No Public Risk Labels** → the student view never displays risk status.

---

## 5. References

* **Tool 01** – Civitas Learning Student Success Platform. Analyzed October 2026. See file `01 - Tool Analysis Civitas Learning & RNL.md`.
* **Tool 02** – EAB Navigate360 Student Success Management System. Analyzed October 2026. See file `02 - Tool Analysis EAB Navigate360 (Analog.md`.
* **Tool 03** – Salesforce Education Cloud / Next-Gen SIS. Analyzed October 2026. See file `03 - Tool Analysis Salesforce Education Cloud.md`.
* **Heuristics** – Nielsen, J. (1994). *10 Usability Heuristics for User Interface Design*. NN/g.
* **Framework** – Garrett, J. J. (2010). *The Elements of User Experience*. New Riders.

---

## 6. Notes

* This document is **Phase 2 only** and was written after the problem statement was defined.
* It supersedes any initial assumptions from Phase 1 in the summary file (`00 - Benchmark Summary`).
* All adopted/rejected patterns are traceable to a specific tool and section in the benchmark.