---
title: Developer guide
has_children: false
nav_order: 11
---

# Developer Guide

This guide explains how to use **PlantAI** from a developer's perspective, including setting up the project, using the software’s API, and building additional features.

## Getting Started

### Prerequisites
Before you begin, ensure you have the following installed:
- **Node.js** (v14 or higher)
- **npm** (v6 or higher)
- An **OpenAI API key**

### Setup

1. **Clone the Repository**:
   - Clone the repository to your local machine:
     ```
     git clone https://github.com/unibo-dtm-se-2324-myplants/artifact.git
     ```

2. **Install Dependencies**:
   - Navigate to the project directory and install the required Node.js dependencies:
     ```
     cd artifact
     npm install
     ```

3. **Configure Environment Variables**:
   - Create a `.env` file in the root of the project and add your OpenAI API key:
     ```
     OPENAI_API_KEY=your_openai_api_key
     ```

4. **Run the Development Server**:
   - Start the development server locally:
     ```
     npm start
     ```
   - The application will be accessible at `http://localhost:3000`.

## Project Structure

The **PlantAI** project follows a typical Node.js and Express.js structure:

- **server.js**: The entry point for the backend server.
- **public/**: Contains frontend assets like HTML, CSS, and JavaScript.
- **service-worker.js**: Manages offline caching for the frontend.
- **package.json**: Contains the project metadata and dependencies.

## API Overview

**PlantAI** provides an API endpoint to upload images and retrieve plant identification data. Developers can integrate this API into their own applications to extend the functionality.

### API Endpoints

#### POST `/submit`

This endpoint processes an image upload and returns plant identification data using the OpenAI API.

- **Method**: `POST`
- **Parameters**:
  - `image`: The image file of the plant.
  - `location`: A string indicating if the plant is "indoor" or "outdoor".
  
- **Response**:
  - On success, the server responds with a JSON object containing:
    - `commonName`: A random name for the plant.
    - `scientificName`: The scientific name of the plant.
    - `wateringFrequency`: Number of days between waterings.
    - `description`: A short description of the plant.
    - `careInstructions`: Instructions for caring for the plant.
    - `isPlant`: Boolean indicating if a plant was identified.
