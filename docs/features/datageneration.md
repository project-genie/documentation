---
sidebar_position: 5
---

# Data Generation

We needed a dataset to train our machine learning model yet we cannot find a appropriate one for us.

Then we decided to create our dataset using existing APIs and similar datasets.

We created a python script to get data from external sources and create ours.

The python repository is here: https://github.com/project-genie/python-database-composer-script

First, we create 20 *users*, the random user data is fetched from this api: https://randomuser.me/api/

Secondly, we create 200 *tasks*, the random task name and difficulty is created in the python code. They don't matter much.

Then, we create 200 *completed_tasks* referencing the *tasks* table. Here we use the "difficulty" property to generate a *completed_date* for tasks. When the difficulty is higher, the completed_date is also a bit longer.

