---
title: FlowIntel 3.3.0 - Task-to-object link, Stability Refinements... 
description: We are pleased to announce FlowIntel 3.3.0, introducing a new feature, Task-to-object link. This release focuses on strengthening the connectivity between your investigation data and refining the user interface experience.
author:
 - David Cruciani
date: 2026-05-21
---

## Flowintel 3.3.0 (2026-05-21)

We are pleased to announce FlowIntel 3.3.0, introducing a new feature, **Task-to-object link**. This release focuses on strengthening the connectivity between your investigation data and refining the user interface experience.

---

### 🚀 New Features

*   **Task-to-Object Linking:** You can now directly link tasks to specific objects within a case, providing a tighter association between your analysis steps and the evidence involved.
<img width="1631" height="464" alt="objects" src="https://github.com/user-attachments/assets/c15261ff-f0a8-4f53-b2cb-52ee3b7a8dde" />
<img width="1598" height="564" alt="Screenshot from 2026-05-21 10-22-35" src="https://github.com/user-attachments/assets/d49854cd-4137-45d6-9f83-c7d67f6452c5" />

---

### 🛠 Improvements & Changes

*   **Modernizing the Frontend:** Continued the transition to **Vue.js** for the Chatbot and Alerting modules, including a comprehensive refactor of `v-cloak` to eliminate "Flash of Uncompiled Content" (FOUC) issues.
*   **Pivotick Integration:** Updated to the latest version of the Pivotick library to ensure better stability and timeline rendering.
*   **Case Consistency:** Standardized terminology and labels throughout the application for a more cohesive user experience.
*   **Templates & Workflow:** Case templates now properly include notes, and version numbering has been extended to cases and tasks for better change tracking.
*   **Admin & Permissions:** Improved visibility into permission requirements; users are now explicitly notified when they lack the required admin rights to modify taxonomies or galaxies.

---

### 🐞 Bug Fixes

*   **Security & Access:** Prevented unauthorized forks of privileged cases and ensured that case-level alerts respect private case access permissions.
*   **Task Management:** Refined the task "revive" logic to prevent unintended status resets after a task is marked as finished.
*   **Stability:** Fixed various JavaScript and Vue compilation warnings, ensured history directories are created during installation, and resolved minor UI glitches in the Note and Analyser tabs.
*   **Audit Logging:** Fixed timezone synchronization issues in audit log graphs for accurate activity reporting.

---

### 📖 Documentation
*   Updated the user manual with fresh screenshots and comprehensive documentation for the latest architectural changes.

## Contributors

- @cudeso 
- @ecrou-exact



**Full Changelog**: https://github.com/flowintel/flowintel/compare/3.2.0...3.3.0

---

# Funding

Flowintel is co-funded by [CIRCL](https://www.circl.lu/) and by the European Union under [FETTA](https://www.circl.lu/pub/press/20240131/) (Federated European Team for Threat Analysis) project.

![EU logo](https://www.vulnerability-lookup.org/images/eu-funded.jpg)
