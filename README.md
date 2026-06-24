# APPorte - Volunteer Coordination in Climate Emergencies

## Table of Contents

1. [Project Identification](#1-project-identification)
2. [The Problem](#2-the-problem)
3. [Scope of the Solution / Proposal Description](#3-scope-of-the-solution--proposal-description)
4. [UX Elements Layer](#4-ux-elements-layer)
   - [4.1. Strategy](#41-strategy)
   - [4.2. Scope](#42-scope)
   - [4.3. Structure](#43-structure)
   - [4.4. Skeleton](#44-skeleton)
   - [4.5. Surface](#45-surface)
5. [Benchmark Analysis](#5-benchmark-analysis)
6. [UX Personas](#6-ux-personas)
7. [Value Proposition Canvas](#7-value-proposition-canvas)
8. [Navigability Flow](#8-navigability-flow)
9. [Low-Fidelity Proposal](#9-low-fidelity-proposal)
10. [Interface Evolution & Justification](#10-interface-evolution--justification)
11. [High-Definition Interfaces & Interactive Prototype](#11-high-definition-interfaces--interactive-prototype)
12. [Heuristic Evaluation](#12-heuristic-evaluation)
13. [Accessibility Considerations](#13-accessibility-considerations)
14. [Device Navigation Evidence](#14-device-navigation-evidence)
15. [Design Critiques Received (Presentation I)](#15-design-critiques-received-presentation-i)

---


## 1. Project Identification

**Course:** User Experience Design and Human-Computer Interaction (UXD-HCI), 2026
**Institution:** Universidad de La Frontera (UFRO), Department of Computer Science.

**Team Members & Roles:**

- **Project Manager:** Luis Jaramillo - Responsible for project leadership, team cohesion, general planning, and presentations.
- **Analyst:** Vicente Salazar - Responsible for the interview process, user needs conceptualization, and data organization.
- **Designer:** Felipe Seguel - Responsible for formal deliverable models, low-fidelity wireframes, and high-definition interfaces.

---

## 2. The Problem

During climate emergencies such as wildfires and floods in the Araucanía region, volunteer brigades face massive coordination chaos. Currently, the operation relies heavily on standard, non-specialized communication apps like WhatsApp. This methodology leads to overlapping tasks, communication breakdowns, and critical information loss, heavily hindering response efforts and efficient resource allocation in high-stress environments.

---

## 3. Scope of the Solution / Proposal Description

**APPorte** is a centralized digital hub designed to transform emergency response through strict coordination. The application offers a data-driven platform that provides real-time visibility of volunteers and material resources. By consolidating communication and task management, APPorte ensures timely actions, skill-matching squad assignments, dynamic heat maps, and a centralized resource inventory, significantly reducing the cognitive load on volunteers and coordinators.

---

## 4. UX Elements Layer

The UX Research and design phases were structured using Jesse James Garrett's 5 UX Elements framework. Each plane below is explicitly tied to the evidence that produced it: the three UX Personas (Section 6), the Value Proposition Canvas (Section 7), and the Competitive Benchmark (Section 5).

### 4.1. Strategy

From the **project perspective**, APPorte's objective is to replace the improvised use of generic messaging apps (WhatsApp/Telegram) with a single, purpose-built coordination tool for volunteer brigades. This is not an assumption: our own Benchmark Analysis (Section 5) profiled WhatsApp/Telegram directly and confirmed that critical resource and location information gets buried inside chronological chat history — the exact mechanism behind the "information loss" named in our problem statement.

From the **user perspective**, Strategy is built around the three UX Personas: Carlos Morales (a displaced resident who needs fast access to resources), Claudio Cáceres (a volunteer leader who needs rapid, structured visibility over tasks and supplies), and Sebastián Sandoval (a stressed first responder who needs a zero learning curve). All three share one validated need: decisions must be made in seconds, under physical and cognitive stress, without prior training. This is also the central gap our benchmark identified — none of the four tools analyzed (Moviliza-T, Chile Alerta, Waze, WhatsApp/Telegram) combine structured coordination with zero onboarding friction.

### 4.2. Scope

Each functionality below is traceable to a specific persona need or a specific benchmark finding, not an arbitrary feature list:

- **Geolocation-based emergency feed (Foro):** addresses Sebastián's need for zero-friction triage. Adopted Chile Alerta's flat, one-tap navigation pattern; explicitly rejected Moviliza-T's structure, which buries its map behind an "Entities" menu.
- **Interactive Live Heat Map:** addresses Carlos's need for immediate spatial awareness. Adopted Waze's and Chile Alerta's color-coded marker convention (red/blue/yellow), since both demonstrated that color alone communicates urgency faster than text under stress.
- **Specialized Squad Chat with embedded resource tracking:** directly replaces the free-text, unstructured coordination pattern identified as the root cause of duplicated tasks in our WhatsApp/Telegram benchmark profile.
- **Dynamic creation of Collection Points (Acopios) with automated location mapping:** removes manual address typing, rejecting the "cognitive load from long texts/coordinates" pattern flagged in our own benchmark findings.
- **Profile settings with mental health considerations (Active/Inactive toggle):** addresses the "extreme stress" pain point mapped in the Value Proposition Canvas (Section 7).

### 4.3. Structure

The information architecture is designed for linear, fast-response navigation. The user flow is structured around a central Home (Foro) that branches intuitively into localized modules: the Interactive Map, the Account Management dashboard, and the Collection Points (Acopios). Complex decision trees were flattened to ensure that users reach critical data (e.g., needed resources, navigation routes) in three taps or fewer — a target adopted directly from Chile Alerta's bottom-tab structure in our benchmark (Section 5), the only one of the four tools analyzed that reached critical information in a single tap.

> 🔲 **PENDING:** This section's diagram (Section 8) is being revised based on Presentation I feedback — the navigation logic itself needs a clearer, more explicit explanation, not just an updated picture. This text will be expanded once the design lead finalizes the revised flow.

### 4.4. Skeleton

Low-fidelity mockups prioritized content placement and rapid readability. The interface skeleton relies on large, tap-friendly areas, clear visual hierarchies, and progressive disclosure of information to prevent users from being overwhelmed by data in high-stress scenarios. This is a deliberate rejection of two patterns identified in our benchmark: Moviliza-T's dense legal/informational text blocks, and WhatsApp/Telegram's reliance on long free-text messages and manually typed coordinates — both replaced here with iconography, structured fields, and one-tap actions.

### 4.5. Surface

The high-definition interfaces were designed focusing on high contrast and legibility under adverse conditions (e.g., outdoors, smoke, stress).

- **Typography:** *Inter*, selected for its exceptional clarity and readability on mobile devices.
- **Colorimetry:** A structured palette utilizing primary action blues (`#2563eb`), neutral and clean grays for backgrounds (`#f0f2f5`, `#fefefe`) to reduce eye strain, and high-contrast red alerts specifically reserved for critical emergency markers.
- **Language Constraint:** While this documentation is in English, all High-Definition User Interfaces are exclusively in Spanish to cater accurately to the target demographic in La Araucanía.
- See **Section 13 (Accessibility Considerations)** for how these surface-level decisions connect to broader accessibility commitments.

---

## 5. Benchmark Analysis

A two-phase competitive benchmark was conducted to analyze current coordination tools, covering all three required categories plus the incumbent baseline:

| Tool | Category |
|---|---|
| Moviliza-T | Direct competitor |
| Chile Alerta | Analogous competitor |
| Waze | Design reference |
| WhatsApp / Telegram | Incumbent / analogous (named directly in our own problem statement) |

The full written analysis — including the 8 base dimensions, 4 domain-specific dimensions, the synthetic comparative table with the "APPorte (Proposal)" row, and the explicit Adopted/Rejected design decisions — is available in [`APPorte_Benchmark_ENGLISH-POSTcORRECTIONS.pdf`](./assets/APPorte_Benchmark_ENGLISH-POSTcORRECTIONS.pdf).

A complementary Increase/Reduce/Include/Remove decision matrix focused specifically on WhatsApp/Telegram is available in [`APPorte_Benchmark.png`](./assets/APPorte_Benchmark.png).

> 🔲 **PENDING:** Annotated screenshots (minimum 3 per tool, with title + visual annotation + 2-line justification each) — [add folder/link here].
> 🔲 **PENDING:** Feature Map (Standard / Differentiating / Opportunity classification, built collaboratively in FigJam) — [add FigJam export/link here].

---

## 6. UX Personas

Based on our data collection, we identified three core target users affected by the problem:

1. **Carlos Morales (45):** A temporarily relocated victim in a shelter who urgently needs to find reconstruction resources.
2. **Claudio Caceres (25):** An overwhelmed volunteer leader who demands fast responses and efficient data organization.
3. **Sebastian Sandoval (30):** A stressed first responder who is not highly tech-savvy and requires extremely simple, intuitive interfaces.

Detailed profiles can be found in the repository (`UserUX1.jpg`, `UserUX2.jpg`, `UserUX3.jpg`).

---

## 7. Value Proposition Canvas

The development of APPorte is grounded in a thorough Value Proposition Canvas analysis. By mapping user pains (complex systems, extreme stress, duplicated efforts) against gains (helping the community effectively), we built an interface focused on relief. The application directly addresses these pains by ordering elements by proximity and offering real-time inventory tracking. The complete canvas is available in `canvasvalor-apporte.jpg`.

---

## 8. Navigability Flow

The end-to-end user journey illustrates the complete workflow from receiving an emergency alert to task completion. The structural flow navigates from the main Home (Foro) through conditional interactions (e.g., authentication checks) into specialized dashboards, map views, and administrative tools for Collection Points. The current diagram is available in `diagrama_inicial.png`.

> 🔲 **PENDING:** This diagram and its written explanation are being revised by the design lead based on Presentation I feedback ("the process/flow logic was not understood"). The updated version must explain *why* the flow is structured this way, not only show it — [replace link once finalized].

---

## 9. Low-Fidelity Proposal

Initial mockups were created on paper to iterate rapidly over the structural placement of elements without focusing on aesthetics. These digitized sketches served as the foundation for our usability discussions. Files can be reviewed in `Wireframe_Papel.pdf` and `wireframe_papel_2.pdf`. The corrected, fully annotated version — with a Functional Overview and Key Components & Detailed Logic for every screen — is available in [`Wireframe APPorte-PostCorrection.pdf`](./assets/Wireframe%20APPorte-PostCorrection.pdf).

---

## 10. Interface Evolution & Justification

Transitioning from Low-Fi wireframes to High-Definition interfaces required critical modifications based on our UX Research:

- **Foro / Home Feed:** The initial low-fi mockup was a basic list. Recognizing that users need fast decisions under stress, the HD version evolved to order everything by distance automatically. Clear visual tags ('Incendio', 'Inundación', 'Acopio') and distance indicators were added so volunteers know exactly where help is needed first.
- **Interactive Map:** Early wireframes featured simple black pins on a blank space, failing to resolve the "complex systems" pain point. The HD design integrated a real map interface with color-coded markers (red for emergencies, blue for volunteers, yellow for alerts), granting users immediate spatial awareness and an intuitive understanding of the scenario.
- **Squad Chat (Brigada):** To solve communication collapse, the chat screen was evolved to embed a 'Resource Summary' directly inside the conversation. Instead of losing information in text messages, volunteers can visually track supply percentages (e.g., 75% clothes, 30% water), directly eliminating task duplication.
- **Acopio Detail:** Wireframe details were basic. The HD version expanded the 'Needed right now' section with quick visual chips (e.g., 'Agua x50'). Massive, clear buttons for 'Cómo llegar' and 'Chat' were added to make the workflow seamless and reduce cognitive load.
- **Nuevo Acopio:** Standard text inputs were replaced with large, tappable buttons for 'Permanent' or 'Temporal' points. A mini-map was integrated to grab the current location automatically with one tap, recognizing that manually typing a full address during a crisis is impractical.
- **Account & Settings:** Acknowledging the mental toll of volunteering identified in the Canvas, the HD profile prioritized a large 'Active Volunteer' toggle. This allows users to pause critical alerts and assignments when they need to rest, granting them control and peace of mind.

---

## 11. High-Definition Interfaces & Interactive Prototype

The final, refined User Interfaces incorporate community best practices, utilizing the aforementioned typography and colorimetry.

**Interactive Prototype:** <https://www.figma.com/proto/6YhWg90TUEXsVdqo0yeKLw/UX-UI?node-id=172-986&p=f&t=tzWWa902V0H5Qy3j-1&scaling=min-zoom&content-scaling=fixed&page-id=142%3A194&starting-point-node-id=172%3A986&show-proto-sidebar=1>

Exported HD frames are also available in [`HdFRAMEapporte.pdf`](./assets/HdFRAMEapporte.pdf), for evaluators who prefer a static reference alongside the navigable prototype.

> 🔲 **PENDING:** Confirm this link reflects the corrections currently being made (Alerta de Foco screen, address input, Acopio info paddings) before final submission.

---

## 12. Heuristic Evaluation

As part of the course's "Taller 5: Evaluación Heurística" methodology, each group both evaluates another team's project and receives an evaluation of their own. Two reports are relevant here:

- **Evaluation conducted by our team** (on a peer project, "InterBus"), following the standard Severity × Frequency = Criticality framework: [`Informe Euristica.pdf`](./assets/Informe%20Euristica.pdf).
- **Evaluation received from peers, of APPorte itself** (Stephanie Mercado and Felipe Medina), covering 14 distinct usability problems mapped to Nielsen's heuristics with severity/frequency scoring: [`Ev Euristica Recibed`](./assets/EVeuristicaRecibida.pdf).

Every issue identified in the second report has been logged and cross-referenced against the in-class handwritten peer review — see "Design Critiques Received" below.

---

## 13. Accessibility Considerations

Accessibility research for this project was grounded in the course's accessibility workshop, which analyzed real-world digital accessibility initiatives (screen-reader compatibility, multilingual labeling, manual and automated audits) in an existing large-scale platform. The full analysis is available in [`Presentación - Accesibilidad Digital en MercadoLibre.pdf`](<./assets/Presentación - Accesibilidad Digital en MercadoLibre.pdf>).

These principles directly inform APPorte's own accessibility commitments (see Section 4.5, Surface):

- High-contrast color coding reserved specifically for critical alerts, so severity is recognizable without reading text.
- Large, tap-friendly touch targets sized for use under physical stress (e.g., gloved hands, outdoor conditions).
- Icon-first communication patterns that reduce reliance on reading under cognitive load, consistent with the workshop's finding that screen-reader and icon-based navigation benefit users with visual and motor disabilities.

---

## 14. Device Navigation Evidence

> 🔲 **PENDING:** Per the Presentation II rubric, this section must include a screenshot or short video showing APPorte's interfaces running on an actual mobile device (or browser, if web-based), demonstrating full navigation between screens. Waiting on the finalized Figma corrections before recording — [add screenshot/video link here].

---

## 15. Design Critiques Received (Presentation I)

This is the consolidated feedback received on APPorte's interfaces during the Presentation I cross-review, combining handwritten in-class annotations from the peer review session and the formal heuristic evaluation conducted by classmates Stephanie Mercado and Felipe Medina.

### Foro / Home

- Color palette is too flat/plain; lacks a clear visual identity.
- The "Distancia" sort control doesn't read as tappable.
- Navbar is missing shortcuts to frequent destinations (e.g. Chats, Mis Acopios).
- Header says 3 acopios while "Mis Acopios" shows 2 active; the quick view should show active items, with totals in the detail view.
- Spelling: missing accents (e.g. "Pucón"), several "-ción" words missing tildes.

### Acopio Detail (Vista General de un Acopio)

- Category chips (Agua, Alimentos, Ropa, Medicam.) look static; unclear how they get populated when an alert is created, since the creation form doesn't ask for them.
- Unclear whether custom attributes support multiple values.
- Quantities shown here (e.g. "Agua x50") have no matching input field in the creation form.
- Urgency shown as "Urgente" doesn't map clearly to the creation form's Normal / Alto / Crítico options.
- "Total 8/10" doesn't reconcile with the per-category numbers shown elsewhere (12/15, 2/5, 12/15).

### Mapa

- No marker shows the user's own current location.
- Unclear what happens if a referenced location (e.g. Villarrica) isn't covered by the map.

### Nueva Alerta

- Relationship between "Nueva Alerta" and the Foro / map point concept is unclear.
- Screen feels visually empty; layout needs better information distribution.

### Alerta de Foco (Evacuar Zona 2)

- Large empty space between sender info and "Confirmar Recibido."
- That space could hold a small map of the affected zone instead of being empty.
- "¿Qué es zona 2?" / "¿Qué carretera?" — zone and street references aren't specific enough to act on.
- Heavy use of red feels visually invasive, even though it's appropriate for urgency.
- Suggestion: add a fire/hazard icon for faster visual recognition.
- Wording: consider "Confirmar Recibo" instead of "Confirmar Recibido."

### Nuevo Acopio (Step 1 & 2)

- No input field for "Dirección" — the label exists but there's nothing to type into.
- Button color logic unclear ("why transparent black?").
- No date fields for "Temporal" points.
- Unclear who is allowed to create a new Acopio.
- Categories should be a dropdown/standard list, not free text typed by the user.
- Missing a per-category quantity field — the form only captures the category tag, not "how much."
- Phone number field only accepts the literal "+569" prefix, which is too rigid.
- A volunteer can currently create an Acopio and become its responsible contact, even though the role definitions say only Coordinators manage zones.

### Squad Chat (Grupo Brigada)

- Unclear who requested/sent the "Resumen de Recursos" card.
- Real volunteer brigades coordinate by radio, not by chat — the underlying assumption behind this feature was questioned directly.

### Login

- Background image works well.
- Background image feels decontextualized from the emergency-response theme.

### Registro Coordinador

- Unclear whether example field content (e.g. "Camila Rojas") is placeholder text or accidentally pre-filled data.
- Consent text is usually presented as plain text, not wrapped inside a checkbox component this way.

### Account / Profile

- No way to log out from Profile or Settings.
- Resources can only be added — there's no way to edit, decrease, or delete them once created.
