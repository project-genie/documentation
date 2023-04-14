---
sidebar_position: 6
---

# AI Support

Project is equipped with AI features and day by day we add another AI feature to improve usability.

## Task Prediction

We created a dataset and trained our machine learning model.

Then we created a python microservice with this machine learning model and connected the endpoint to our Node.js web server.

When you create a task your user level and task diffuculty information is sent to AI endpoint with this information .
AI calculates working hours for the task. Then creates the task on the database with an estimated date.

Repo of the AI is here: https://github.com/project-genie/python-ai