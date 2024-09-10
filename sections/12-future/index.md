---
title: Future work
has_children: false
nav_order: 13
---


# Known Issues and Future Work

## Known Issues

1. **Vercel Deployment Challenges**:
   - **Issue**: The application could not be fully deployed on Vercel due to challenges with the integration of the backend, service worker caching, and the OpenAI API.
   - **Impact**: This prevents the live version of the app from functioning as expected in a cloud environment. Currently, the app can only be run locally.
   - **Potential Fix**: Exploring other deployment platforms or refactoring the backend to better align with Vercel’s serverless architecture might resolve these issues.

2. **Service Worker Cache Management**:
   - **Issue**: The service worker is set up to cache essential files for offline use, but it occasionally fails to update or cache new assets correctly after a deployment. This could lead to outdated versions of the app being served to users.
   - **Impact**: Users might experience inconsistent offline behavior or encounter issues when using the app offline after an update.
   - **Potential Fix**: Improving the service worker's cache invalidation strategy and adding more granular control over asset updates could resolve this issue.

3. **Handling Large Image Files**:
   - **Issue**: The current implementation doesn’t efficiently handle large image files, leading to longer processing times or, in some cases, timeouts.
   - **Impact**: Users with large images may experience delays, and the backend may struggle to process the request efficiently.
   - **Potential Fix**: Implementing image compression before sending the file to the OpenAI API or adding size limitations to the upload process can mitigate this problem.

4. **Limited Plant Database**:
   - **Issue**: The current identification relies solely on the OpenAI API, which may not always provide accurate or detailed information for all plant types.
   - **Impact**: Some users may not receive the level of detail they expect, and certain rare or less common plants might not be recognized.
   - **Potential Fix**: Expanding the backend to include a more extensive plant database or integrating additional APIs specifically focused on plant identification could improve accuracy and breadth of plant data.

## Missing Features

1. **User Authentication and Profile Management**:
   - **What’s Missing**: Currently, there is no system for user authentication or profile management. All data is stored locally in the browser.
   - **Impact**: Users cannot save or access their plant data across different devices.
   - **Future Work**: Implementing a user authentication system, possibly with cloud-based data storage, would allow users to manage their plant care profiles across devices.

2. **Advanced Plant Care Features**:
   - **What’s Missing**: The app provides basic care instructions, but it doesn’t account for specific user environments like humidity, soil type, or regional weather conditions.
   - **Impact**: Care instructions are generalized and might not fully reflect the user’s local environment.
   - **Future Work**: Integrating weather and environmental APIs to customize plant care advice based on the user's location and local conditions.

3. **Push Notifications for Watering Reminders**:
   - **What’s Missing**: While notifications are implemented, they rely on local browser permissions and may not work as expected across all devices or if the app is not open.
   - **Impact**: Users may miss critical watering reminders if notifications are blocked or not functioning properly.
   - **Future Work**: Implementing a more robust push notification system, possibly with a backend service to send reminders even when the app is closed, could improve this feature.

## Future Work

1. **Refactor to Next.js**:
   - **Why**: Moving the app to **Next.js** would provide better server-side rendering capabilities, simplify the deployment process (especially on platforms like Vercel), and improve overall performance.
   - **Benefits**: This would likely resolve the current deployment challenges, improve SEO for public-facing pages, and provide better scalability.

2. **Database Integration with MongoDB**:
   - **Why**: Integrating **MongoDB** would allow for more robust data management by offering a flexible schema to store plant information and user-specific care schedules.
   - **Benefits**: This would improve data reliability, enabling users to store their plant data securely, sync it across devices, and retrieve it efficiently. MongoDB’s NoSQL structure would also allow the app to scale as more users and plant species are added, while ensuring detailed, context-specific plant care information is easily accessible.

3. **Mobile Application Development**:
   - **Why**: Given that many users will likely want to identify plants while on the go, a native mobile application (iOS/Android) would provide a more seamless and accessible experience.
   - **Benefits**: A mobile app would enable users to capture plant images directly from their phone’s camera and receive plant care reminders in a more integrated fashion.

4. **Gamification Features**:
   - **Why**: Adding gamification elements to the app would increase user engagement and provide an enjoyable learning experience about plant care.
   - **Benefits**: Users could earn badges or points for correctly identifying plants, keeping up with watering schedules, or caring for a variety of plants. Leaderboards or achievement systems could foster a community of plant enthusiasts and encourage regular use of the app.

---

By addressing these known issues and expanding the app with these future developments, **PlantAI** can evolve into a more robust, user-friendly, and feature-rich platform for plant enthusiasts.
