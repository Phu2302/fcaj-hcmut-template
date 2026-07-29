---
title: "Week 4 Worklog"
date: 2024-01-01
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
reportTableColumns:
  - Day
  - Task
  - Completion Date
reportType: worklog
---

### Week 4 Objectives:

* Start Backend development: implement core APIs for the LMS project.
* Set up local DynamoDB environment and connect it with the server.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Clone repository to local machine, install dependencies.<br>- Configure environment variables (`.env`) for MySQL and DynamoDB.<br>- Run local server and test `/health` endpoint. | 06/07/2026 | 06/07/2026 | |
| 3 | - Build login/registration API using JWT.<br>- Create User model and authentication middleware.<br>- Test API with Postman: `POST /auth/login`, `POST /users`. | 07/07/2026 | 07/07/2026 | |
| 4 | - Develop Classes & Courses API: `GET`, `POST`, `PUT`, `DELETE`.<br>- Write Class and Course models, query DynamoDB with GSI.<br>- Run `seed_sample_data.sh` script to populate sample data. | 08/07/2026 | 08/07/2026 | |
| 5 | - Develop Schedules & Grades API.<br>- Design StudentSchedule table schema.<br>- Write controllers and routes for schedule and grade viewing features. | 09/07/2026 | 09/07/2026 | |
| 6 | - Code review developed APIs, fix bugs, and optimize.<br>- Team meeting to check progress and plan for Week 5. | 10/07/2026 | 10/07/2026 | |


### Week 4 Achievements:

* Backend runs stably on local environment with DynamoDB and MySQL.
* Completed foundational APIs: Auth, Users, Classes, Courses, Schedules, Grades.
* Database populated with sample data, ready for testing and Frontend development.
