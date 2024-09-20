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
   - Image upload and identification should complete within a reasonable time (e.g., within 5 seconds under normal conditions).  
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
  
## Dependencies

- **dotenv** (`^16.4.5`): Used to load environment variables from a `.env` file into `process.env` for secure configuration management.
  
- **express** (`^4.19.2`): A web framework for Node.js, used to handle HTTP requests and build the backend server.

- **multer** (`^1.4.5-lts.1`): Middleware for handling multipart/form-data, specifically for uploading plant images.

- **openai** (`^4.45.0`): Used to interact with the OpenAI API for plant image identification and care recommendations.

## Explanation of Terms

1. **Service Worker**  
   **Definition**: A script that runs in the background, separate from a web page, enabling features such as offline capabilities and push notifications.  
   **Usage in PlantAI**: Used to cache essential files, ensuring the app works offline and can send notifications.
