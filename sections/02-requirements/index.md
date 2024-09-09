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
   - If the image is not of a plant, the application should notify the user appropriately (e.g., "Plant not recognized").

3. **Watering Schedule Generation**  
   The application must generate a watering schedule based on the identified plant type and its environment (indoor/outdoor).  
   - Users can specify whether the plant is indoor or outdoor.  
   - The application provides a recommended watering frequency based on the plant's type and environment.

4. **Notification System**  
   The application must remind users to water their plants according to the schedule generated.  
   - Users can enable notifications for watering reminders.  
   - The application sends timely notifications to users to remind them to water their plants.

5. **Image Upload and Response Storage**  
  The application must allow users to upload images and store past responses for future reference.  
   - Users can drag and drop or select an image file to upload.  
   - The application stores past identifications and watering schedules locally for easy access and review.

6. **Offline Functionality**  
   The application must function offline by caching necessary resources and maintaining access to stored data.  
   - Users can access the application and view past responses even without an internet connection.  
   - The service worker caches essential files (e.g., HTML, CSS, JavaScript, images) to allow offline operation.

## Non-functional Requirements

1. **Performance**  
   The application should process images and retrieve responses quickly to provide a smooth user experience.  
   - Image upload and identification should complete within a reasonable time (e.g., within 10 seconds under normal conditions).  
   - Notifications should be timely and occur without delays.

2. **Usability**  
   The application should have an intuitive and user-friendly interface.  
   - Users should be able to easily upload images and receive plant identification results with minimal effort.  
   - The interface should be clean, responsive, and easy to navigate.

3. **Security**  
   The application must handle user data, especially images, securely to protect privacy.  
   - All user data should be securely transmitted and stored, complying with data protection regulations.

4. **Reliability**  
   The application should be reliable and available whenever users need it.  
   - The application should maintain high availability (e.g., 99% uptime or higher).  
   - The notification system should consistently remind users to water their plants.

## Implementation Requirements

1. **Programming Languages**  
    The application must be developed using specific programming languages and frameworks.  
   - The frontend should be developed using HTML, CSS, and JavaScript.  
   - The backend should be developed using Node.js and Express.

2. **APIs and Libraries**  
    The application must utilize specific APIs and libraries for image processing and AI capabilities.  
   - The OpenAI API should be used for plant identification and analysis.  
   - Multer should be used for handling image file uploads on the server side.

3. **Tools and Platforms**  
   The application should use specified tools and platforms for development and deployment.  
   - The application should be hosted on a cloud platform (e.g., AWS, Heroku, or Vercel).  
   - Git should be used for version control.  
   - Docker may be used for containerization and consistent deployment.

## Explanation of Terms

1. **Service Worker**  
   **Definition**: A script that runs in the background, separate from a web page, enabling features such as offline capabilities and push notifications.  
   **Usage in PlantAI**: Used to cache essential files, ensuring the app works offline and can send notifications.

2. **Multer**  
   **Definition**: A middleware for Node.js used for handling multipart/form-data, primarily for uploading files.  
   **Usage in PlantAI**: Used on the server side to handle image uploads from users.

3. **OpenAI API**  
   **Definition**: A platform provided by OpenAI offering AI capabilities such as natural language processing and image recognition.  
   **Usage in PlantAI**: Used to analyze uploaded plant images and provide identification and care instructions.

---

By adhering to these requirements, "PlantAI" will provide a feature-rich, secure, and reliable application that meets user needs for plant identification, care tracking, and notification reminders.









# Requirements

- The requirements must explain what the application will have to do. You should not focus on the particular problems, but exclusively on what you want the application to do

- Goals must be clearly explained

- Requirements are divided into:
    - **Functional**: describe the actual behaviour of the application
    - **Non-functional**: requirements that do not directly concern behavioural aspects, such as safety, performance, etc.
    - **Implementation**: constrain the entire phase of system realization, for instance by requiring the use of a specific programming language and/or a specific software tool.

- If there are unclear terms (ambiguous, very complex, etc.) these should be explained
- Each requirement must have its own acceptance criteria

