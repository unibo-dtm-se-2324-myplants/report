---
title: Design
has_children: false
nav_order: 4
---

# Design

## Architecture
The architecture of "PlantAI" follows a **layered architecture**, ensuring modularity and maintainability. The key layers include:

1. **Presentation Layer**: Handles the user interface using HTML, CSS, and JavaScript. Manages user interactions and communicates with the backend via HTTP requests.
2. **Business Logic Layer**: Built with Express.js, this layer processes user requests, applies business rules, and coordinates interactions between other layers.
3. **Data Access Layer**: Manages data storage and retrieval. Local storage is used for caching responses on the client, while Multer handles image uploads on the server.
4. **Service Layer**: Interfaces with external services like the OpenAI API to perform plant identification.

## Modelling


## Interaction
When a user uploads an image, the system follows this flow:
1. The image is uploaded via the frontend.
2. A request is made to the backend to process the image.
3. The backend sends the image to the OpenAI API for identification.
4. Once a response is received, the plant data is displayed to the user, and past responses are stored locally.

![image](https://github.com/user-attachments/assets/2482758f-45fb-4c26-8a9b-21e923525614)

## Behaviour
The system transitions through the following states:
1. **Initial State**: No image uploaded.
2. **Processing**: After an image is uploaded and is being analyzed.
3. **Result Displayed**: After a successful plant identification.
4. **Error State**: If the system fails to identify a plant or encounters an error.

![image](https://github.com/user-attachments/assets/f85a5f29-9841-4824-8b01-5d98816d0e81)

## Data-related Aspects
The application uses **Local Storage** for caching user data and responses, ensuring offline access. **Multer** is employed to handle image uploads on the server, and these images are sent to the OpenAI API for plant identification.

![Screenshot 2024-09-09 173143](https://github.com/user-attachments/assets/23977adb-6125-4301-8c7e-6f0ef2e5029b)


## Domain-driven Design (DDD)
The system is designed with clear **bounded contexts** for managing user data and plant responses. **Repositories** abstract data access from local storage, and **services** handle plant identification and notifications. The design respects **hexagonal architecture**, ensuring separation of concerns between domain logic and external systems.

![Eventstorming](Eventstorming.png)
