---
title: Development
has_children: false
nav_order: 5
---

# Development

## DVCS (Distributed Version Control System)

For the development of **PlantAI**, Git was used as the distributed version control system, with GitHub serving as the repository host. Below are the key practices followed throughout the project:

### Branching Conventions

- **Main Branch**:
  - **Purpose**: The main branch (`main` or `master`) holds the stable version of the project. Only thoroughly tested and reviewed changes are merged into this branch.
  - **Usage**: Direct commits to the main branch are avoided. All new features, bug fixes, and enhancements are developed in separate branches and only merged into the main branch after a successful pull request (PR) review.

- **PWA Branch**:
  - **Purpose**: A separate branch for Progressive Web App (PWA) features. This branch focuses on implementing offline functionality, caching strategies, and service worker management.
  - **Usage**: Changes related to PWA features are developed here and merged into the main branch once verified.

**Personal Workflow**: Initially, I found the concept of branches new and challenging. Working solo on a small project, I often relied on local backup versions and uploaded stable versions directly to GitHub. However, moving forward, I plan to leverage Git branches more effectively for managing feature development and bug fixes.

### Commit Conventions

PlantAI follows the **Conventional Commits** standard to maintain a clear and consistent commit history. The structure of commit messages follows this format:

#### Types of Commits:
- **feat**: Introduces a new feature.
- **fix**: Fixes a bug.
- **docs**: Changes to documentation.
- **style**: Code style changes that do not affect functionality (e.g., formatting).
- **refactor**: Code changes that neither fix a bug nor add a feature.
- **perf**: Performance improvements.
- **test**: Adding or correcting tests.

#### Example Commit Messages:
- fix(noplant-detected): error message removed after 5 seconds
- feat(notification): watering for each plant
- docs(manifest): added

#### Frequency and Granularity:
- **Atomic Commits**: Changes are committed frequently in small, self-contained units to make it easier to understand the project history and revert changes if needed.
- **Granularity**: Each commit represents a single logical change, such as adding a feature, fixing a bug, or updating documentation.

---

## Implementation Details

## Personal Learnings and Growth

Throughout the development of **PlantAI**, I experienced significant personal growth in my technical abilities. Prior to this project, I was unfamiliar with several key technologies, but by tackling the challenges presented, I gained a much deeper understanding of how to build a complex, fully functional application.

### Key Learnings:

#### Using OpenAI API for Image Recognition
- **Challenge**: Before this project, I had limited experience integrating third-party APIs, especially for tasks like image recognition.
- **What I Learned**: By working with the OpenAI API, I gained insights into structuring API requests, handling image data (like converting images to base64), and managing asynchronous processes. I also learned to work with multipart form-data for image uploads, a skill that will be incredibly useful for future projects.
- **Outcome**: Integrating AI-powered plant identification was a major achievement. It gave me confidence in using cutting-edge technologies to enhance user experience, and I now have a much stronger foundation in working with APIs.

#### AI-Powered Development and Problem Solving
- **Challenge**: Working on certain areas of the project, like image recognition and managing client-side storage, was initially overwhelming. I wasn’t sure how to approach some of these advanced concepts.
- **What I Learned**: AI tools and resources played a crucial role in my learning process. Not only did AI help with debugging and solving complex problems, but it also guided me in understanding new programming concepts and applying them correctly.
- **Outcome**: With the support of AI and persistent learning, I was able to achieve things that seemed out of reach at the start of this journey. This project has truly opened my eyes to how AI can enhance productivity and learning, especially when tackling challenging development tasks.

### Proud of the Progress
I'm incredibly proud of how far I’ve come with **PlantAI**. From using Git effectively for version control to integrating advanced features like AI-powered plant identification and offline functionality, this project has been a profound learning experience. Each new technology I mastered — from service workers to the OpenAI API — represents a step forward in my journey as a developer. 

Working on this project has taught me not just about code, but about perseverance, creativity, and leveraging modern tools, including AI, to solve problems and build something meaningful.
