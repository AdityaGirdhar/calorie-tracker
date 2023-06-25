# Calorie Tracking REST API

## Getting started

### Installating Dependancies
Developers using this project must have [python3](https://www.python.org/downloads/) and [pip](https://pip.pypa.io/en/stable/installation/) installed.

This project uses a virtual environment (venv) to isolate dependancies and prevent version conflicts (optional, but recommended). If you're using a python virtual environment as well, open your terminal and run:

```
source backend/{env-name}/bin/activate
``` 
(assuming `env-name` is the name of your virtual environment)

Once your virtual environment is ready, run:

```
pip install -r backend/requirements.txt
```

## Running the server

Before proceeding ensure that your virtual environment has been activated. Not doing so can lead to messy module import errors. To run the app, open yor terminal and run:

```
python backend/app.py
```

## API Reference

### Overview
* Base URL: The backend is assumed to be hosted at `http://127.0.0.1:5000`.
* Authentication: This section will be updated as authentication support is added

For a complete API reference, refer to `backend/README.md`.

## Assumptions/Choices
1 . The requirement document says

> "a regular user would only be able to CRUD on their owned records, a user manager would be able to CRUD only users, and an admin would be able to CRUD all records and users."

It's slightly ambiguous as to whether a manager can CRUD another manager or not, but for the purpose of this project I have assumed they can't.

## Citations and References
Here is a (non-exhaustive) list of online resources I referred to while working on this project.

- Flask Documentation (v2.3.x) - [https://flask.palletsprojects.com/en/2.3.x/](https://flask.palletsprojects.com/en/2.3.x/)
- SQLAlchemy 2.0 Documentation - [https://docs.sqlalchemy.org/en/20/](https://docs.sqlalchemy.org/en/20/)
- Role-based Access Control (RBAC) in REST APIs - [https://medium.com/@BastianRob/rbac-in-rest-api-b6ed65d1f4d8](https://medium.com/@BastianRob/rbac-in-rest-api-b6ed65d1f4d8)
