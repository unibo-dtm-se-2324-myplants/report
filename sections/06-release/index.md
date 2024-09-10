---
title: Release
has_children: false
nav_order: 7
---

# Release

## What to Release, Where, and How

### What to Release:
The primary release of **PlantAI** will include:
- **Frontend**: The complete web application with offline capabilities, including all HTML, CSS, and JavaScript files.
- **Backend**: The Node.js server with integration to the OpenAI API, including all server-side code, API handlers, and image processing logic.
- **Service Worker**: Configured for caching resources and enabling offline functionality.
- **Documentation**: Comprehensive README files covering setup instructions, deployment guidelines, and API usage details.

### Where to Release:
- **GitHub**: The codebase will be made available as an open-source project on GitHub, allowing for easy access, contribution, and issue tracking.
- **Vercel (or similar platform)**: The live version of **PlantAI** will be deployed on a cloud platform such as Vercel for users to experience the full functionality, including plant identification and notification features.

However, during development, I encountered some challenges deploying this version of the app on **Vercel**, particularly related to handling the backend integration and service worker caching. If I had to start over, I would consider using **Next.js**. Next.js offers better support for server-side rendering, more seamless integration with Vercel, and optimized deployment workflows. By switching to Next.js, I believe the development process would be smoother, especially for managing server-side logic and improving the overall performance of the app.

### How to Release:
1. **Pre-Release Testing**: Before releasing the final version, ensure thorough testing of all features, especially offline functionality, image uploads, and API interactions.
2. **Deployment**: Deploy the application using a continuous deployment pipeline through Vercel or another platform, linking to the latest tagged version.
3. **Versioning**: Follow semantic versioning for future updates, ensuring clear communication of major changes, fixes, or enhancements.

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

### Why SemVer?
- **Seen in class documentation**
- **Clarity**: It clearly indicates the type of changes in each release, helping users and contributors understand the impact of updates.
- **Predictability**: Developers can confidently update the application knowing that backward-compatible versions won’t break existing functionality.
- **Industry Standard**: Semantic versioning is widely used and understood in the open-source community, making it easier for contributors to follow the project's evolution.

---

This release plan ensures **PlantAI** is accessible, well-maintained, and ready for future enhancements while following best practices for versioning and licensing.


