---
title: Deployment
has_children: false
nav_order: 8
---

# Deployment

## Local

To deploy **PlantAI** and ensure it works seamlessly locally on users' machines, follow these steps:

1. **Clone the Repository**:
   - Clone the repository from GitHub using:
     ```
     git clone https://github.com/unibo-dtm-se-2324-myplants/artifact.git
     ```

2. **Install Dependencies**:
   - Navigate to the project directory and install the required dependencies:
     ```
     cd plantai
     npm install
     ```

3. **Environment Variables**:
   - Set up the necessary environment variables. Create a `.env` file in the root of the project and add the following:
     ```
     OPENAI_API_KEY=your_openai_api_key
     ```

4. **Run the Application**:
   - Start the server locally:
     ```
     npm start
     ```

These operations will ensure that **PlantAI** is fully functional and ready for both local development.

---

## Live

The live version of **PlantAI** will be deployed on a cloud platform such as Vercel for users to experience the full functionality, including plant identification and notification features.

However, during development, I encountered some challenges deploying this version of the app on **Vercel**, particularly related to handling the backend integration and service worker caching. Initially, I attempted to deploy the app on **Heroku**, but after investing both time and money, the results were not as expected.

That’s when I decided to rely on **Vercel** that is free for small projects. If I had to start over, I would also consider using the **Next.js** framework. Next.js offers better support for server-side rendering, more seamless integration with Vercel, and optimized deployment workflows. By switching to Next.js, I believe the development process would be smoother, especially for managing server-side logic and improving the overall performance of the app.

So due to these deployment challenges, the online version is currently unavailable.
