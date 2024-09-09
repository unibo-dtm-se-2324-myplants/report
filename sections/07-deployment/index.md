---
title: Deployment
has_children: false
nav_order: 8
---

# Deployment
# Deployment

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

### Vercel Deployment Challenges
While attempting to deploy **PlantAI** to Vercel, I encountered several issues, particularly related to handling service worker caching and backend integration with the OpenAI API. Due to these deployment challenges, the online version is currently unavailable. If I were to start over, I would consider using **Next.js** for better compatibility with Vercel's deployment environment, which could help avoid these issues.
