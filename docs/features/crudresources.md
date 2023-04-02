---
sidebar_position: 4
---

# CRUD Resources

## Organization

Organization is the top resource in the application. Without creating the organization, user cannot perform any actions.

Organization routes are in path _/api/organizations_.

We have functions on this route that enables user to fetch all the organizations they are member of, create, update, or delete organizations.

## Project

One organization can have one or many projects. And these routes resides at _/api/projects_.

Only the organization owner can create, update, or delete projects. This authorization is provided by access tokens (they are sent along with the requests).

We also have routes that enables users to fetch the projects that they are a member of.

## Task

One project can have one or many tasks. These routes are at _/api/tasks_

All members in a project can create tasks. But only the owner of the task can update, or delete the task.
