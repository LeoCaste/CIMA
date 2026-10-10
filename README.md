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
  - [4.3. Dual-Track Customer Journey Map](#43-dual-track-customer-journey-map)
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

#### Claudio Novarro — Academic Director
* **Goal:** Early, confidential intervention without stigmatizing students. 
* **Needs:** Clear risk dashboards with explicit uncertainty indicators.
[![UX Persona - Claudio Novarro](https://github.com/user-attachments/assets/bbbcf2eb-7c02-4dbc-9fd5-e85ca9b9ac3f)](files/ux_persons/claudio_novarro.pdf)

#### José Pérez — First-Year Student
* **Goal:** Track grades while privately obtaining academic help. 
* **Needs:** A non-judgmental portal to request discrete tutoring.
[![UX Persona - José Pérez](https://github.com/user-attachments/assets/c426c1d9-b9cb-46f4-b301-02fcec9bb581)](files/ux_persons/jose_perez.pdf)

#### León Castillo — Peer Tutor
* **Goal:** Help junior students and reduce help-seeking friction. 
* **Needs:** A privacy-preserving mechanism to receive tutoring requests.
[![UX Persona - León Castillo](https://github.com/user-attachments/assets/f26b729f-0395-4b28-a614-4e59554c3ecc)](files/ux_persons/leon_castillo.pdf)

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

📄 **[View the Complete Competitive Benchmark Analysis (PDF)](files/benchmark/Benchmark.pdf)**

#### Feature Map
The feature map defines our market differentiators, including our unique approach to qualitative certainty wording and discreet help channels. Click the image to view the PDF version.

[![Feature Map](https://github.com/user-attachments/assets/a6487db1-d0e8-4daa-8bd6-24abd7a8ec0c)](files/benchmark/assets/feature_map.pdf)

#### Comparative Matrix
The evaluation covers 9 core UX dimensions. *Note: Dimensions 4, 5, and 6 correspond directly to the domain-specific criteria evaluated in this project.* Click the image to view the PDF version.

[![Comparative Matrix](https://github.com/user-attachments/assets/0f68e9cd-d15d-48ea-bb1b-e295d8fc4e46)](files/benchmark/assets/comparative_matrix.pdf)

### 4.3. Dual-Track Customer Journey Map

Traditional Early Warning Systems map only the administrative flow, ignoring the psychological impact on the student. To ensure CIMA remains empathetic and non-stigmatizing, we developed a **Dual-Track Customer Journey Map** to define the necessary touchpoints and interaction requirements before structuring the application.

This map explicitly traces the emotional and actionable parallel paths of both Claudio (Academic Director) and José (First-Year Student), demonstrating the exact moment where the system cross-contacts them without public exposure.

* **Claudio's Track:** Moves from the tension of evaluating a risk alert to the satisfaction of executing a contextual, empathetic outreach without disciplinary friction.
* **José's Track:** Moves from the anxiety of academic struggles to the relief of receiving a supportive message, culminating in the empowerment of using the discreet self-request channel for tutoring.

**📄 [View the Dual-Track Customer Journey Map (PDF)](files/Customer_journey_map.pdf)**
