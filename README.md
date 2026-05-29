# Application Features

## Main Dashboard

Upon logging in, the user sees the main dashboard with key information:

- Current date and day of the week
- Number of today's appointments and all scheduled appointments (for the logged-in doctor/medical staff)
- Personal data of the logged-in user, their role, and specialties

Available options include:
- Theme selection (light/dark)
- Full-screen mode

<img width="2557" height="1390" alt="image" src="https://github.com/user-attachments/assets/3c104d7b-2f33-4144-a36d-5831de0f643d" />
<br><br>
<img width="1919" height="1078" alt="dashboard_main" src="https://github.com/user-attachments/assets/54d55a8c-827e-4ae3-85dd-9ba0640e2ced" />

## Patients Module

Manages patient data, diagnoses, and prescriptions.

- The patient list includes: first name, last name, PESEL (National ID), phone, email, address, date of birth, and status
- The list of diagnoses and prescriptions contains linked patient information
- Ability to add, update, and delete patients, diagnoses, and prescriptions
- Access depends on the user's role (medical staff only have access to their own patients)

<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/d2d3ea5c-bced-45eb-ba65-ef3715390f46" />
<br><br>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/c94f5313-1d9d-4d67-b9ec-077e6708ad2b" />

## Employees Module

Manages employee data, their services, and specialties.

- Employee list with basic contact details and activity status
- List of services and specialties assigned to employees
- Tables mapping services and specialties facilitate workflow organization
- Add, update, and delete operations are available to roles: administrator, receptionist, IT specialist, and manager

<img width="1918" height="1079" alt="serv_spec_CRUD" src="https://github.com/user-attachments/assets/9006cd99-feb7-4ec9-a263-c2dd61011a59" />
<br><br>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/7ad8d902-a71f-451f-9108-1368ae806967" />

## Rooms and Reservations Module

Manages rooms and reservations.

- Room list including room number, floor, and type
- Reservation list with date, time, room number, and reservation type
- Ability to add, update, and delete rooms, room types, and reservations
- Access granted to all roles except the guest role

<img width="1915" height="1079" alt="rooms_CRUD" src="https://github.com/user-attachments/assets/e299f0a1-a5b3-46b6-a041-da59cc15bb70" />
<br><br>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/3d7bdeb6-60e4-457e-950f-f5b7ca040df3" />

## Schedule Module

Manages appointments and internal meetings.

- The appointment list includes patient data, employee, service, room, date, time, notes, and appointment status
- List of meeting types and internal meetings
- Ability to add, update, and delete meetings and participants
- All operations available to roles except the guest role

<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/3430c1b6-2fb7-4e58-8938-b4718030231c" />
<br><br>
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/008367d3-7792-4c30-b19e-81799495c082" />

## Administrative Settings Module

The most restricted module, accessible only to the Administrator and IT Specialist.

- Management of users, roles, and patient-to-staff assignments
- Full access to add, update, and delete users and assignments
- Crucial for the authorization system and patient care organization

<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/13156eec-0b5d-4f2e-82df-27347ff7fb8c" />
<br><br>
<img width="1919" height="1079" alt="prezentacja_roles_list" src="https://github.com/user-attachments/assets/3e7c318b-5b74-4f78-a480-b2342a237801" />

---

# README — Running the Project

Below is a comprehensive guide on how to run the project locally and how to build the `.exe` file. The instructions assume a Windows environment and a Python installation outside of the Microsoft Store.
**Important**: work within a virtual environment (`venv`) — this is the best practice.

## Requirements
- Python **3.11.9**
- OS: Windows (instructions include PowerShell commands)
- Installed packages (use the `requirements.txt` file)

## `requirements.txt` Content

Create a `requirements.txt` file in your repository containing the exact versions (example):

```text
altgraph==0.17.4
astroid==3.3.5
bcrypt==5.0.0
colorama==0.4.6
coverage==7.6.7
dill==0.3.9
greenlet==3.1.1
iniconfig==2.0.0
isort==5.13.2
mccabe==0.7.0
mypy==1.13.0
mypy-extensions==1.0.0
mysql-connector-python==9.1.0
packaging==24.2
pefile==2023.2.7
pip==24.0
platformdirs==4.3.6
pluggy==1.5.0
pyinstaller==6.16.0
pyinstaller-hooks-contrib==2025.9
pylint==3.3.1
pylint-pytest==1.1.8
PyQt6==6.7.1
PyQt6-Qt6==6.7.3
PyQt6_sip==13.8.0
PyQt6-WebEngine==6.7.0
PyQt6-WebEngine-Qt6==6.7.3
PyQt6-WebEngineSubwheel-Qt6==6.7.3
PySide6==6.8.0.2
PySide6_Addons==6.8.0.2
PySide6-DS==4.6
PySide6_Essentials==6.8.0.2
pytest==8.2.0
pytest-cov==6.0.0
pytest-faulthandler==2.0.1
pytest-sugar==1.0.0
pywin32-ctypes==0.2.3
setuptools==65.5.0
shiboken6==6.8.0.2
SQLAlchemy==2.0.36
termcolor==2.5.0
tomlkit==0.13.2
typing_extensions==4.12.2
