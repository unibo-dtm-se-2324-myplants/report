---
title: Home
layout: home
has_children: false
nav_order: 1
---

# PlantAI

### Authors
- [Domenico Copia](mailto:domenico.copia@studio.unibo.it)

## Abstract

The project aims to create a **Progressive Web App (PWA)** that allows users to upload images of their houseplants and receive detailed information on each plant’s scientific name and watering schedule. The app is designed to be user-friendly, providing seamless access to plant care instructions and reminders through a combination of client-side and server-side functionalities.

From the **client side**, users can perform several key tasks:
- **Upload images** of plants to identify them and save plant care data.
- **Access a personalized section** that lists all previously saved plants, complete with their care instructions.
- **Receive notifications** that remind them when it’s time to water their plants based on the provided schedule.

The **server side**, developed using **Node.js**, manages communications with the **OpenAI API** to perform image classification and plant identification. When a user uploads an image, the server sends the image to the API for analysis, processes the response, and returns detailed information about the plant, including its name and care instructions.

To enhance user experience, the application is designed to store plant data locally using browser storage functionalities. This enables users to access their saved plants and care information even when offline. Additionally, the PWA supports offline functionality through the implementation of a **service worker**, ensuring that essential assets are cached and available even without an internet connection.

Overall, this project provides a convenient tool for plant owners, combining AI-powered plant identification with practical, personalized plant care management in an easily accessible PWA format. Future enhancements may include advanced features like user accounts, cloud storage, and integration with external APIs for more accurate and location-specific care advice.
