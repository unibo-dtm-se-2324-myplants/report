---
title: Requirements
has_children: false
nav_order: 3
---

# Requirements

## Functional Requirements

1. **Plant Identification**  
   The application must be able to identify plants from images uploaded by the user and provide relevant details.  
   - Users can upload an image of a plant.  
   - The application processes the image and returns the plant’s common name, scientific name, care instructions, and watering schedule.  
   - If the image is not of a plant, the application notifies the user appropriately with "Plant not recognized."

   **Acceptance Criteria:**  
   - Users can successfully upload plant images and receive identification results.  
   - The identification results should include the plant's common name, scientific name, care instructions, and watering schedule.
   - If the image is not a plant, the user is notified with a clear error message, and no data is returned.

2. **Watering Schedule Generation**  
   The application must generate a watering schedule based on the identified plant type and its environment (indoor/outdoor).  
   - Users can specify whether the plant is indoor or outdoor.  
   - The application provides a recommended watering frequency based on the plant's type and environment.

   **Acceptance Criteria:**  
   - Users can select whether a plant is indoor or outdoor.  
   - The watering schedule returned must be based on the plant type and environment with an appropriate frequency (e.g., days between watering).

3. **Notification System**  
   The application must remind users to water their plants according to the schedule generated.  
   - Users can enable notifications for watering reminders.  
   - The application sends timely notifications to users to remind them to water their plants.

   **Acceptance Criteria:**  
   - Notifications are sent at the correct time intervals based on the watering schedule generated.  
   - Users receive notifications even when the app is not actively being used.

4. **Image Upload and Response Storage**  
   The application must allow users to upload images and store past responses for future reference.  
   - Users can drag and drop or select an image file to upload.  
   - The application stores past identifications and watering schedules locally for easy access and review.

   **Acceptance Criteria:**  
   - Users can upload images using both drag-and-drop and file selection.  
   - Past identifications and responses are saved and can be reviewed even after the session ends.

5. **Offline Functionality**  
   The application must function offline by caching necessary resources and maintaining access to stored data.  
   - Users can access the application and view past responses even without an internet connection.  
   - The service worker caches essential files (e.g., HTML, CSS, JavaScript, images) to allow offline operation.

   **Acceptance Criteria:**  
   - The application can load essential pages and display previously stored responses while offline.  
   - Cached resources allow the application to function without an active internet connection.

## Non-functional Requirements

1. **Performance**  
   The application should process images and retrieve responses quickly to provide a smooth user experience.  
   - Image upload and identification should complete within a reasonable time (e.g., within 5 seconds under normal conditions).  
   - Notifications should be timely and occur without delays.

   **Acceptance Criteria:**  
   - The system should be able to process image uploads and return results in under 5 seconds for most users.  
   - Notifications should be sent no later than 10 seconds after the scheduled time.

2. **Usability**  
   The application should have an intuitive and user-friendly interface.  
   - Users should be able to easily upload images and receive plant identification results with minimal effort.  
   - The interface should be clean, responsive, and easy to navigate.

   **Acceptance Criteria:**  
   - Users can complete core tasks (upload image, view results) with minimal instruction.  
   - The interface should render correctly across different devices and screen sizes.

3. **Security**  
   The application must handle user data, especially images, securely to protect privacy.  
   - All user data should be securely transmitted and stored, complying with data protection regulations.

   **Acceptance Criteria:**  
   - All image uploads and data transfers should use secure HTTPS encryption.  
   - The application should not expose any sensitive data, and all user data should be stored securely.

4. **Reliability**  
   The application should be reliable and available whenever users need it.  
   - The application should maintain high availability (e.g., 99% uptime or higher).  
   - The notification system should consistently remind users to water their plants.

   **Acceptance Criteria:**  
   - The application should demonstrate 99% uptime over any given month.  
   - Notifications should consistently function without missed reminders.

## Implementation Requirements

1. **Backend API**  
   The application must have a backend that processes image uploads and handles requests for plant identification.  
   - Develop RESTful APIs using a scalable framework like Node.js to handle image processing and communicate with external APIs (e.g., OpenAI for plant identification).  

   **Acceptance Criteria:**  
   - APIs should be well-documented and adhere to REST principles, allowing seamless integration with the frontend.  
   - The API should process and respond to image upload requests within 5 seconds under normal conditions.

2. **Frontend Development**  
   The frontend should be developed using modern UI principles to provide a responsive user interface.  
   - The user interface must be intuitive and support both mobile and desktop devices.  

   **Acceptance Criteria:**  
   - The frontend should adapt gracefully to different screen sizes and orientations, ensuring cross-browser compatibility.  
   - Users should be able to upload images, view plant identifications, and receive notifications on both mobile and desktop devices.

3. **Notification System**  
   Implement a notification system using the browser’s `Notification API` and service workers.  
   - Notifications should be scheduled based on the plant’s watering schedule and delivered even when the app is not actively being used.  

   **Acceptance Criteria:**  
   - Notifications should be sent at the correct times according to the watering schedule, regardless of whether the user is actively using the app.  

4. **Offline Functionality**  
   The application must cache essential files and responses for offline use.  
   - Use service workers to cache the necessary assets (e.g., HTML, CSS, JS, images) and store previous identifications locally for offline access.  

   **Acceptance Criteria:**  
   - The application should function offline, displaying cached content and stored responses.  
   - Service worker audits should confirm that the necessary assets are cached correctly for offline usage.

## Explanation of Terms

1. **Service Worker**  
   **Definition**: A script that runs in the background, separate from a web page, enabling features such as offline capabilities and push notifications.  
   **Usage in PlantAI**: Used to cache essential files, ensuring the app works offline and can send notifications.
