# TaskManagerAPI
# Task Manager API

Overview
TaskManagerAPI is a RESTful API built with Flask and SQLAlchemy that allows users to manage tasks more efficiently. The API allows you to add, retrieve, update, and delete tasks stored in a SQLite database.

Features
- Add new tasks
- Retrieve all tasks
- Update existing tasks (including marking as completed)
- Delete tasks
- SQLite database for persistent storage

Tech Used
- Python
- Flask
- Flask-SQLAlchemy
- SQLite
- Git & GitHub for version control

Installation

*Prerequisites*
Ensure you have Python and `pip` installed on your system.

##Clone the Repository

git clone https://github.com/Hord16/TaskManagerAPI.git
cd TaskManagerAPI


##Create and Activate Virtual Environment

python3 -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

##Install Dependencies

pip install -r requirements.txt

##Run the Application
---
python3 app.py
---

## API Endpoints

*Base URL*
---
http://127.0.0.1:5000
---

##Get All Tasks
*Endpoint:* `GET /tasks`
---
curl http://127.0.0.1:5000/tasks
---

##Add a Task
*Endpoint:* `POST /tasks`
---
curl -X POST http://127.0.0.1:5000/tasks -H "Content-Type: application/json" -d '{"title": "Learn Flask"}'
---

##Update a Task
**Endpoint:** `PUT /tasks/<id>`
---
curl -X PUT http://127.0.0.1:5000/tasks/1 -H "Content-Type: application/json" -d '{"completed": true}'
---

##Delete a Task
*Endpoint:* `DELETE /tasks/<id>`
---
curl -X DELETE http://127.0.0.1:5000/tasks/1
---

## Contributing
Feel free to fork the repository and submit pull requests with improvements!

## License


