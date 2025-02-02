# azure-diagram-onlinelearningplatform

********************
Task: 
Scenario 2: Online Learning Platform

Architecture:
1. Presentation Tier (Frontend):
  - Components:Web browser, Mobile app.
  - Technologies:Angular, HTML, CSS, JavaScript, Flutter (for mobile apps).
2. Application Tier (Backend):
  - Components:Web server, API server.
  - Technologies:Python with Django/Flask, Ruby on Rails, Node.js.
3. Data Tier (Database):
  - Components:** Database server, File storage.
  - Technologies:** PostgreSQL (for relational data), Amazon S3/Google Cloud Storage (for storing course materials).
Scenario:
An online learning platform where users can enroll in courses, watch video lectures, and complete assignments.
- User Interaction:Users interact with the website or mobile app to browse courses, watch videos, and submit assignments.
- Business Logic:The backend server manages user authentication, course enrollment, and assignment submissions.
- Data Storage:Course details, user progress, video files, and assignment submissions are stored in the database and file storage.
Flow:
1. The user logs in to the online learning platform via the website or mobile app.
2. The frontend requests course data from the backend.
3. The backend retrieves course information from the database and sends it to the frontend.
4. The user enrolls in a course and starts watching video lectures.
5. The backend tracks the user's progress and stores it in the database.
6. The user submits assignments, which are processed by the backend and stored.
********************

Diagram:
![Azure - Scenario 2](https://github.com/user-attachments/assets/a2d3c69e-5fd3-46fa-9953-f44a6a999859)

Explanation: 2 regions used to ensure high availability and to be fault tolerant

- Azure Traffic Manager is a DNS-based traffic load balancer that distributes traffic optimally to services across global Azure regions while providing high availability and responsiveness.
- Azure load balancer used to spread load across availability zones
- Virtual machines used for web and app servers
- PostgreSQL databases used for relational data
