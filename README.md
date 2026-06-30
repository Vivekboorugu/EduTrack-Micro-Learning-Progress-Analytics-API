# EduTrack — Micro-Learning Progress & Analytics API

This project is a REST API built with FastAPI, SQLModel, and SQLite, utilizing a clean Service Layer Architecture.

## Setup Instructions

### 1. Create a Virtual Environment (Recommended)
Before installing dependencies, it is best practice to create an isolated Python environment:

    python -m venv venv

    # On Windows:
    venv\Scripts\activate
    # On macOS/Linux:
    source venv/bin/activate


### 2. Install Dependencies
Ensure the `requirements.txt` file is in your current directory and run:

    pip install -r requirements.txt


### 3. Initialize the Database and Run the Server
You do not need to run a separate script to create the database. The application is configured to automatically generate the SQLite database file (`microlearning.db`) and seed it with initial data the first time you boot the server.

Start the FastAPI application using Uvicorn:

    uvicorn main:app --reload


### 4. Access the Interactive API Documentation
Once the server is running, you can interact with all endpoints (enrollments, completing lessons, dashboard, and leaderboards) via the automatically generated Swagger UI:
* **Interactive Docs:** [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
