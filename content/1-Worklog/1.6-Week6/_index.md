---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
reportTableColumns:
  - Day
  - Task
  - Completion Date
reportType: worklog
---

### Week 6 Objectives:

* Deploy the entire application onto AWS infrastructure.
* Configure domain and CI/CD to automate deployment workflows.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 2 | - Deploy Backend to EC2: install Node.js, PM2, clone repo.<br>- Configure environment variables (`.env`) for production.<br>- Verify Backend status via public IP. | 20/07/2026 | 20/07/2026 | |
| 3 | - Build Frontend with Vite: `npm run build`.<br>- Upload build artifacts to S3 bucket.<br>- Configure S3 static website hosting. | 21/07/2026 | 21/07/2026 | |
| 4 | - Set up CloudFront distribution pointing to S3 bucket.<br>- Configure CORS between Frontend (CloudFront) and Backend (EC2).<br>- Test complete application on production environment. | 22/07/2026 | 22/07/2026 | |
| 5 | - Configure AWS DynamoDB (replacing local instance).<br>- Run `setup_dynamodb.sh` and `seed_sample_data.sh` scripts on production environment.<br>- Verify Backend → AWS DynamoDB connectivity. | 23/07/2026 | 23/07/2026 | |
| 6 | - Set up basic CI/CD with GitHub Actions: auto-deploy on code push.<br>- End-to-end testing: login, view courses, attempt quizzes, submit assignments.<br>- Log and resolve issues arising on production. | 24/07/2026 | 24/07/2026 | |


### Week 6 Achievements:

* LMS application running completely on AWS: Frontend via CloudFront, Backend on EC2, data on DynamoDB.
* CI/CD pipeline fully operational, auto-deploying code updates seamlessly.
* All features operating reliably on production environment.
