---
title: Concept
has_children: false
nav_order: 2
---

# Concept

**Product Type:**
The project developed is a web application with a graphical user interface (GUI). This type of product is designed to be accessible from web browsers, making it platform-independent and easy to use for a wide range of users. The main functionalities are implemented and accessible through a user-friendly web interface, which includes forms, buttons, and visual feedback to interact with the user.

## Idea

The idea for "MyPlant" comes from two primary motivations: my personal interest in houseplant care and my passion for the rapidly evolving field of generative AI. My goal was to create a practical and user-friendly app for plant enthusiasts that could be financially sustainable.

## Market Analysis

To understand the market landscape, I reviewed several popular plant care and identification apps available on the Google Play Store. Here are some notable examples and their download counts:

- **PictureThis:** 50M downloads
- **PlantNet Plant Identification:** 10M downloads
- **Flora Incognita:** 5M downloads
- **PlantIN:** 5M downloads
- **Blossom:** 5M downloads
- **Plantum:** 1M downloads
- **Planta:** 1M downloads
- **Seek by iNaturalist:** 1M downloads

These numbers clearly indicate a strong market demand for plant identification and care apps, confirming the potential for "MyPlant."

## Business Model Understanding

To build a sustainable app, I analyzed the revenue models of existing applications. Most of these apps generate income through subscription models, with average prices around $30 for the whole year or $7 for one month only. This pricing strategy aligns well with the cost structure for using the OpenAI ChatGPT model for plant identification.

### Cost Analysis of OpenAI Usage:

- **GPT-4 Turbo:** $0.012 per request (based on my requests data, in line with the price per token on the OpenAI platform)
- **GPT-O:** $0.0056 per request (based on my requests data, in line with the price per token on the OpenAI platform)

With an average cost of approximately half a cent per identification request, using OpenAI’s API is financially viable. Assuming an annual subscription fee of $30 and accounting for 50% in taxes and other costs, we have a net revenue of $15 per user per year. This translates to supporting up to 3000 identifications per year, or about 250 per month, which is significantly higher than the expected usage by an average user.

Given these numbers, it is feasible to run a profitable app using OpenAI’s API for plant identification, provided that users maintain an active internet connection for the service.

## Market Positioning

Entering a highly competitive market requires a unique value proposition. To differentiate "MyPlant" from other similar apps, I plan to incorporate gamification elements. This approach will help the app stand out, attract a broader audience, and increase user engagement by making plant care more interactive and enjoyable.

Although the gamification features are not yet implemented, they form the foundation for a separate future development. Detailed plans for gamification will be documented separately.

## Features:

### Image Upload and Recognition:

- Users can upload images of their plants either by dragging and dropping the image file or by selecting it from their device.
- The application uses an AI model to analyze the uploaded image and identify the plant.

### Watering Schedule:

- Based on the identified plant, the application provides a recommended watering schedule.
- Users can specify if the plant is indoor or outdoor, which may affect the watering frequency.

### Local Storage of Responses:

- The application saves the user's past plant identifications and watering schedules locally, allowing them to view their history and keep track of multiple plants.

### Notifications:

- The application requests permission to send notifications.
- Users receive reminders when it's time to water their plants based on the provided schedule.

### Offline Functionality:

- The application uses a service worker to cache resources, allowing it to function offline or in low-connectivity situations.

## Use Case Collection:

### Houseplant Enthusiasts:

- Individuals who have a collection of houseplants and need assistance in identifying and caring for them.
- They can use the app to ensure their plants are watered on time and are healthy.

### New Plant Owners:

- People who are new to owning plants and may not be familiar with the care requirements.
- The app provides guidance on how often to water their plants, which is especially useful for beginners.

### Educational Purposes:

- Teachers or educators in botany or biology can use the app as a teaching tool to help students learn about different plant species and their care requirements.

### Gardeners:

- Gardeners who manage both indoor and outdoor plants can benefit from the app’s ability to provide tailored watering schedules based on the environment.

By combining a user-friendly web interface with powerful AI-driven plant identification and care recommendations, "MyPlant" serves as a comprehensive tool for plant enthusiasts, new plant owners, educators, and professionals alike.


Here you should explain:
- The type of product developed with that project, for example (non-exhaustive):
    - Application (with GUI, be it mobile, web, or desktop)
    - Command-line application (CLI could be used by humans or scripts)
    - Library
    - Web-service(s)
    - Data processing toolkit (= Library + CLI, or Jupyter Notebook)
- Use case collection
