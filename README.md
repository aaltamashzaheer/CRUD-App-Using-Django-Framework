# CRUD-App-Using-Django-Framework <img src="https://icon-icons.com/icons2/2107/PNG/32/file_type_django_icon_130645.png" alt="django-icon" width="30">

This is a web-based application for employee management built with Django. It allows an admin user to perform CRUD (Create, Read, Update, Delete) operations on employee records.

<!-- Add table of contents -->
## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

<!-- Add features list -->
## Features
- User-friendly interface for managing employee data.
- Add, edit, and delete employee information.
- Filter employee data by various attributes such as position.

<!-- Add installation instructions -->
## Installation

To get started with Employee Management System, you need to have Python and pip installed on your system. Then, follow these steps:

1. Clone this repository:
```python
git clone https://github.com/aaltamashzaheer/CRUD-App-Using-Django-Framework
```
2. Navigate to the project directory:
```python
cd CRUD-App-Using-Django-Framework
```
3. Install the required packages:
```python
pip install -r requirements.txt
```
4. Download and Install the Postgres SQL database:
```python
# Download Postgres SQL installer
# Install Postgres SQL by following the installer instructions
```
5. Configure Postgres SQL in settings.py file:
```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'EmployeeDB', #Db name specified in pg admin tool
        'USER': 'postgres', #default user is postgres
        'PASSWORD': 'Altamash123@postgres', #the password you set during installation of Postgres SQL installer
        'HOST': 'localhost', #if we are using DB locally
    }
}
```
6. Apply the database migrations:
```python
python manage.py makemigrations
python manage.py migrate
```
7. To run App migrations:
```python
#To migrate app Tables
python manage.py makemigrations app_name
python manage.py sqlmigrate app_name 0001 #0001 is migration file name

#Migrate all changes to DB:
python manage.py migrate
```
8. Run the development server:
```python
python manage.py runserver
```


The application will now be available at `http://localhost:8000`.

## Usage
Some usage points for this System
1. Easily manage employee data with a user-friendly web interface
2. Add, edit, and delete employee information from a centralized location
3. Keep track of employee performance metrics, such as attendance and productivity

## Contributing

If you would like to contribute to the CRUD APP?
You can follow these steps:

1. Fork this repository.
2. Create a new branch for your feature or bug fix.
3. Write your code and add tests if possible.
4. Submit a pull request.

## License

The Employee Management System is licensed under the MIT License. See [LICENSE](LICENSE) for more information.
