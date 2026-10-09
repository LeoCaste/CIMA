# CIMA - Confidential Intervention & Mentorship Analytics

An empathetic, privacy-first Early Warning System for academic risk management without stigmatization.

---

## Index

- [1. Team Identification and Roles](#1-team-identification-and-roles)
- [2. Problem Statement & Proposed Solution](#2-problem-statement--proposed-solution)
  - [2.1. Problem Statement](#21-problem-statement)
  - [2.2. Solution Overview](#22-solution-overview)
- [3. The Strategy](#3-the-strategy)
  - [3.1. Value Proposition Canvas](#31-value-proposition-canvas)
  - [3.2. UX Personas](#32-ux-personas)
- [4. The Scope](#4-the-scope)
  - [4.1. Scope Delimitation & Justification](#41-scope-delimitation--justification)
  - [4.2. Benchmarking](#42-benchmarking)

---

## 1. Team Identification and Roles

* **Leonardo Castellón** — Team Lead
* **Cristóbal Ramos** — Analyst
* **Héctor Rosales** — UX/UI Designer

---

## 2. Problem Statement & Proposed Solution

### 2.1. Problem Statement
Educational institutions calculate academic risk indicators based on attendance, grades, and platform usage. However, algorithmically labeling a student as "at risk" carries significant social side effects: public stigmatization, self-fulfilling prophecies, and unintended disciplinary actions. 

The challenge involves two main stakeholders with distinct needs—academic directors seeking timely intervention without labeling students, and students seeking discreet support without feeling judged or exposed. Furthermore, the underlying algorithmic model is inherently fallible and contains uncertainty. The design must resolve what information is shown to whom, how algorithmic uncertainty is transparently expressed, and what concrete, empathetic actions are enabled.

### 2.2. Solution Overview
We propose an empathetic, privacy-first academic support platform. Instead of exposing public risk tags or automated disciplinary notices, the solution provides academic directors with uncertainty-aware risk dashboards and non-stigmatizing communication templates. Students gain access to a private self-management portal where they can check their status and discreetly request tutoring support without fear of public exposure.

---

## 3. The Strategy

### 3.1. Value Proposition Canvas
The Value Proposition Canvas bridges user pains/gains with system features, emphasizing algorithmic transparency, discrete support, and non-stigmatizing communication templates.

![Value Proposition Canvas](files/UX-Template-Value-Proposition-Canvas-final.png)

### 3.2. UX Personas
Each persona was developed to map the needs of our three core stakeholders, ensuring that our intervention model focuses on privacy and reduces the friction to seek help.

* **Claudio Novarro (Academic Director):** Goal is early, confidential intervention without stigmatizing students. Needs clear risk dashboards with explicit uncertainty indicators. 
  📄 **[View Persona (PDF)](files/ux_persons/claudio_novarro.pdf)**
* **José Pérez (First-Year Student):** Goal is to track grades while privately obtaining academic help. Needs a non-judgmental portal to request discrete tutoring. 
  📄 **[View Persona (PDF)](files/ux_persons/jose_perez.pdf)**
* **León Castillo (Peer Tutor):** Goal is to help junior students and reduce help-seeking friction. Needs a privacy-preserving mechanism to receive tutoring requests. 
  📄 **[View Persona (PDF)](files/ux_persons/leon_castillo.pdf)**

---

## 4. The Scope

### 4.1. Scope Delimitation & Justification
To maintain architectural consistency, traceability, and prevent functional overload, the system scope is strictly delimited to **one primary flow** and **two secondary flows**.

**Included Flows:**
* **Primary Flow:** *Early Risk Identification & Confidential Empathetic Outreach (Academic Director).* The Academic Director views student risk indicators alongside algorithmic uncertainty levels and initiates contact using predefined templates.
* **Secondary Flow 1:** *Private Academic Status Tracking & Discrete Help Request (Student).* The student accesses a private view of their academic progress and can discretely request assistance.
* **Secondary Flow 2:** *Discrete Tutoring Request Management (Peer Tutor).* Peer tutors receive anonymized tutoring assignments based on subject difficulty patterns.

**Out of Scope (Justification):**
* **Direct Course Teacher View:** Excluded to prevent potential classroom bias, unintentional labeling, and privacy leaks during lectures.
* **Automated Sanctions:** The system deliberately omits automated disciplinary notices or penalty workflows to avoid punitive outcomes.
* **Direct Grade Book Modification:** The platform does not alter institutional grade registers or official transcripts.

### 4.2. Benchmarking
To define the functional boundaries of CIMA and validate our approach to algorithmic uncertainty and privacy, we analyzed existing market solutions (Civitas Learning, EAB Navigate360, and Salesforce Education Cloud). 

The complete breakdown of our findings, adopted/rejected UI patterns, and tool-specific evaluations can be found in our benchmark documentation:

* 📑 **[View Benchmark Summary & Findings](files/benchmark/summary.md)**
* 📊 **[View Feature Map (PDF)](files/benchmark/assets/feature_map.pdf)**
* 📈 **[View Comparative Matrix (PDF)](files/benchmark/assets/comparative_matrix.pdf)**
