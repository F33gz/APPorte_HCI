# APPorte - Volunteer Coordination in Climate Emergencies

## 1. Project Identification
**Course:** User Experience Design and Human-Computer Interaction (UXD-HCI), 2026  
**Institution:** Universidad de La Frontera (UFRO), Department of Computer Science.  

**Team Members & Roles:**
* **Project Manager:** Luis Jaramillo - Responsible for project leadership, team cohesion, general planning, and presentations.
* **Analyst:** Vicente Salazar - Responsible for the interview process, user needs conceptualization, and data organization.
* **Designer:** Felipe Seguel - Responsible for formal deliverable models, low-fidelity wireframes, and high-definition interfaces.

---

## 2. The Problem
During climate emergencies such as wildfires and floods in the Araucanía region, volunteer brigades face massive coordination chaos. Currently, the operation relies heavily on standard, non-specialized communication apps like WhatsApp. This methodology leads to overlapping tasks, communication breakdowns, and critical information loss, heavily hindering response efforts and efficient resource allocation in high-stress environments.

---

## 3. Scope of the Solution / Proposal Description
**APPorte** is a centralized digital hub designed to transform emergency response through strict coordination. The application offers a data-driven platform that provides real-time visibility of volunteers and material resources. By consolidating communication and task management, APPorte ensures timely actions, skill-matching squad assignments, dynamic heat maps, and a centralized resource inventory, significantly reducing the cognitive load on volunteers and coordinators.

---

## 4. UX Elements Layer
The UX Research and design phases were structured using the 5 UX Elements framework:

### 4.1. Strategy
The primary objective is to alleviate the communication collapse and mental burnout experienced by volunteers during crises. The strategy focuses on rapid decision-making, ensuring that user needs—ranging from displaced victims requiring immediate resources to stressed first responders needing clear instructions—are met efficiently without complex technological barriers.

### 4.2. Scope
The application encompasses functionalities designed for rapid deployment:
* Geolocation-based emergency feed (Foro).
* Interactive Live Heat Map for spatial awareness.
* Specialized Squad Chat with embedded resource tracking.
* Dynamic creation of Collection Points (Acopios) using automated location mapping.
* Profile settings with mental health considerations (Active/Inactive availability toggles).

### 4.3. Structure
The information architecture is designed for linear, fast-response navigation. The user flow is structured around a central Home (Foro) that branches intuitively into localized modules: The Interactive Map, the Account Management dashboard, and the Collection Points (Acopios). Complex decision trees were flattened to ensure that users reach critical data (e.g., needed resources, navigation routes) in three taps or fewer.

### 4.4. Skeleton
Low-fidelity mockups prioritized content placement and rapid readability. The interface skeleton relies on large, tap-friendly areas, clear visual hierarchies, and progressive disclosure of information to prevent users from being overwhelmed by data in high-stress scenarios.

### 4.5. Surface
The high-definition interfaces were designed focusing on high contrast and legibility under adverse conditions (e.g., outdoors, smoke, stress). 
* **Typography:** *Inter*, selected for its exceptional clarity and readability on mobile devices.
* **Colorimetry:** A structured palette utilizing primary action blues (`#2563eb`), neutral and clean grays for backgrounds (`#f0f2f5`, `#fefefe`) to reduce eye strain, and high-contrast red alerts specifically reserved for critical emergency markers.
* **Language Constraint:** While this documentation is in English, all High-Definition User Interfaces are exclusively in Spanish to cater accurately to the target demographic in La Araucanía.

---

## 5. Benchmark Analysis
An initial exploration and competitive reference phase was conducted to analyze current coordination tools. The benchmark highlights the limitations of generalized communication apps versus specialized disaster management tools. Detailed annotated screenshots, an idea map, and a synthetic comparative table are available in the repository files (`APPorte_Benchmark.png` and `benchmark A-poorte.pdf`).

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

## 8. Navigability Flow & Customer Journey
The end-to-end user journey illustrates the complete workflow from receiving an emergency alert to task completion. The structural flow navigates from the main Home (Foro) through conditional interactions (e.g., authentication checks) into specialized dashboards, map views, and administrative tools for Collection Points. The complete diagram is available in `diagrama_inicial.png`.

---

## 9. Low-Fidelity Proposal
Initial mockups were created on paper to iterate rapidly over the structural placement of elements without focusing on aesthetics. These digitized sketches served as the foundation for our usability discussions. Files can be reviewed in `Wireframe_Papel.pdf` and `Wireframe APPorte.pdf`.

---

## 10. Interface Evolution & Justification
Transitioning from Low-Fi wireframes to High-Definition interfaces required critical modifications based on our UX Research:

* **Foro / Home Feed:** The initial low-fi mockup was a basic list. Recognizing that users need fast decisions under stress, the HD version evolved to order everything by distance automatically. Clear visual tags ('Incendio', 'Inundación', 'Acopio') and distance indicators were added so volunteers know exactly where help is needed first.
* **Interactive Map:** Early wireframes featured simple black pins on a blank space, failing to resolve the "complex systems" pain point. The HD design integrated a real map interface with color-coded markers (red for emergencies, blue for volunteers, yellow for alerts), granting users immediate spatial awareness and an intuitive understanding of the scenario.
* **Squad Chat (Brigada):** To solve communication collapse, the chat screen was evolved to embed a 'Resource Summary' directly inside the conversation. Instead of losing information in text messages, volunteers can visually track supply percentages (e.g., 75% clothes, 30% water), directly eliminating task duplication.
* **Acopio Detail:** Wireframe details were basic. The HD version expanded the 'Needed right now' section with quick visual chips (e.g., 'Agua x50'). Massive, clear buttons for 'Cómo llegar' and 'Chat' were added to make the workflow seamless and reduce cognitive load.
* **Nuevo Acopio:** Standard text inputs were replaced with large, tappable buttons for 'Permanent' or 'Temporal' points. A mini-map was integrated to grab the current location automatically with one tap, recognizing that manually typing a full address during a crisis is impractical.
* **Account & Settings:** Acknowledging the mental toll of volunteering identified in the Canvas, the HD profile prioritized a large 'Active Volunteer' toggle. This allows users to pause critical alerts and assignments when they need to rest, granting them control and peace of mind.

---

## 11. High-Definition Interfaces & Interactive Prototype
The final, refined User Interfaces incorporate community best practices, utilizing the aforementioned typography and colorimetry. 

**Interactive Prototype:**
https://www.figma.com/proto/6YhWg90TUEXsVdqo0yeKLw/UX-UI?node-id=172-986&p=f&t=tzWWa902V0H5Qy3j-1&scaling=min-zoom&content-scaling=fixed&page-id=142%3A194&starting-point-node-id=172%3A986&show-proto-sidebar=1

