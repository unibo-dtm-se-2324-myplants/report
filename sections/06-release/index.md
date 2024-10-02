---
title: Release
has_children: false
nav_order: 7
---

# Release

### What to Release:
The primary release of **PlantAI** will include:
- **Frontend**: The complete web application with offline capabilities, including all HTML, CSS, and JavaScript files.
- **Backend**: The Node.js server with integration to the OpenAI API, including all server-side code, API handlers, and image processing logic.
- **Service Worker**: Configured for caching resources and enabling offline functionality.
- **Documentation**: Comprehensive README files covering setup instructions, deployment guidelines, and API usage details.
- **NPM Package**: A version of the app's core functionality will also be released as a package on **npmjs.com** to allow developers to integrate PlantAI into their own projects.

### Where to Release:
- **GitHub**: The codebase will be made available as an open-source project on GitHub, allowing for easy access, contribution, and issue tracking.
- **npmjs.com**: The backend and core functionality will be packaged and published as an npm module, allowing for easier distribution and reuse in other projects.

---

## Choice of the License

### License Choice: **MIT License**
The **MIT License** is chosen for **PlantAI** because it provides:
- **Flexibility**: It allows anyone to freely use, modify, and distribute the software without imposing strict conditions.
- **Permissiveness**: Users can incorporate the code into proprietary projects without open-sourcing their own work, encouraging wider adoption and contribution.
- **Simplicity**: The license is short, easy to understand, and widely recognized, making it easier for developers to contribute and use the software.

Given that **PlantAI** is aimed at reaching a broad audience and encouraging contributions, the MIT License is the most suitable choice.

---

## Choice of the Versioning Schema

### Versioning Schema: **Semantic Versioning (SemVer)**
For **PlantAI**, **Semantic Versioning** (SemVer) is chosen because it provides a clear and structured approach to versioning, which will help manage updates and communicate changes effectively. The versioning format will follow this structure:

- **MAJOR**: Incremented for backward-incompatible changes (e.g., major feature rewrites or significant changes in the API).
- **MINOR**: Incremented for backward-compatible new features or enhancements.
- **PATCH**: Incremented for backward-compatible bug fixes or minor improvements.

### What is Being Versioned?
- The **entire codebase** for both frontend and backend.
- Each release will be tagged with a specific version based on **SemVer**, to differentiate between new features, bug fixes, and backward-incompatible changes.

### Why SemVer?
- **Seen in class documentation**
- **Clarity**: It clearly indicates the type of changes in each release, helping users and contributors understand the impact of updates.
- **Predictability**: Developers can confidently update the application knowing that backward-compatible versions won’t break existing functionality.
- **Industry Standard**: Semantic versioning is widely used and understood in the open-source community, making it easier for contributors to follow the project's evolution.

---

### Changelog

### [1.0.0] - May 11, 2024
- **Initial Commit**  
  - Demo import.

### [1.0.1] - May 14, 2024
- **Performance**  
  - Updated to GPT-4o model for plant identification.

### [1.0.2] - May 14, 2024
- **Feature**  
  - Added handling for non-plant images.  
- **Fix**  
  - Fixed form reset after submission.

### [1.0.3] - May 16, 2024
- **Fix**  
  - UI: Response box now appears in a row.  
  - Fixed prompt response wrap issues.
- **Docs**  
  - Added a manifest file for PWA capabilities.

### [1.1.0] - May 17, 2024
- **Feature**  
  - PWA: The app is now installable as a progressive web app.

### [1.1.1] - May 17, 2024
- **Feature**  
  - LocalStorage: Responses are now saved in the browser's local storage.

### [1.1.2] - May 18, 2024
- **Feature**  
  - Notifications: Watering reminders for each plant are now available.  
- **Fix**  
  - No-plant-detected: Error message is removed after 5 seconds.

### [1.1.3] - Sep 09, 2024
- **Fix**  
  - JSON API response: Improved response stability using a more structured JSON format.  
- **Style**  
  - UI improvements, especially on small devices.  
- **Fix**  
  - Minor fix: Comment for notification timeout in seconds.
