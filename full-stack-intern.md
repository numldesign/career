## Full Stack Intern Assignment (5-Hour Task)
This assignment is designed to assess a candidate's skills in **Node.js, Fastify, React, Next.js, PostgreSQL, Drizzle, TypeScript, and Docker** within a manageable timeframe of approximately 5 hours. The task will focus on creating a simple application that incorporates key concepts of system programming, real-time communication, and modern web development practices.

### Task Overview
**Objective:** Build a simple task management application that allows users to create and manage tasks with real-time updates. The application should utilize the latest features of Next.js and React while demonstrating proficiency in backend and frontend development.

### Requirements
**1. Backend Development:**
- Use Node.js with Fastify to create a RESTful API.
- Implement user authentication using JWT (JSON Web Tokens) for a single user (no registration needed; use hardcoded credentials).
- Create a PostgreSQL database schema to store tasks, including fields for task title, description, status (e.g., pending, completed), and timestamps.
- Use Drizzle as an ORM for database interactions.
- Implement basic WebSocket communication for real-time updates when tasks are created or updated.

**2. Frontend Development:**
- Build the frontend using React with the latest features of Next.js, including the app directory structure.
- Create a simple UI that allows users to:
- View a list of tasks.
- Add new tasks with title and description.
- Update the status of tasks (mark as completed).
- See real-time updates when tasks are added or modified by other users (simulated with WebSocket).
- Utilize React’s state management capabilities to handle the application state effectively.

**3. Containerization:**
- Use Docker to containerize both the frontend and backend applications.
- Create a docker-compose.yml file to orchestrate the services (frontend, backend, and PostgreSQL).
- Ensure that all services can communicate effectively within the Docker network.

**4. Testing:**
- Write basic unit tests for critical backend API endpoints.
- Include at least one integration test to ensure that the frontend can successfully interact with the backend API.

**5. Documentation:**
- Provide clear instructions on how to set up and run the application locally using Docker.
- Include brief API documentation detailing endpoints and request/response formats.

### Evaluation Criteria
- **Code Quality:** Cleanliness, organization, and modularity of code.
- **Functionality:** All required features work as expected within the time limit.
- **Performance:** Efficient handling of basic concurrent requests and real-time updates.
- **Testing:** Adequate coverage of unit tests and integration tests.
- **Documentation:** Clarity and completeness of setup instructions and API documentation.

### Deliverables
- Complete source code hosted on a public repository (e.g., GitHub).
- A README.md file with setup instructions and API documentation.
- Docker configuration files for both frontend and backend.

This assignment is intended to take approximately 5 hours to complete. Candidates are encouraged to focus on delivering a functional product while demonstrating their technical skills effectively.
