---
sidebar_position: 1
---

# Run

## 1. Run the Python Flask Application

Make sure that python3 is installed. Installation instructions considered a Windows environment.

1. Clone the repository: `git clone git@github.com:project-genie/python-ai.git`
2. cd into the repository folder. `cd python-ai`
3. Init a virtual environment: `py -3 -m venv venv`
4. Activate the environment: `venv\Scripts\activate`
5. Install the dependencies: `pip install -r requirements.txt`
6. Run the application: `flask --app hello run`

Application serves at: `http://127.0.0.1:5000/`

## 2. Run the Backend Application

Make sure npm is installed on your system.

Make sure that you are running Flask application. It is required for some tasks endpoints.

1. Clone the repository: `git clone git@github.com:project-genie/backend.git`
2. cd into the repository folder: `cd backend`
3. Install the dependencies: `npm i`
4. Run the application: `npm run dev`

Backend serves at: `http://127.0.0.1:8080/`

## 3. Run the Frontend Application

Make sure that you have done requirements above.

1. Clone the repository: `git clone git@github.com:project-genie/frontend.git`
2. cd into the repository folder: `cd frontend`
3. Install the dependencies: `npm i`
4. Run the application: `npm run dev`

Frontend serves at: `http://127.0.0.1:3000/`
