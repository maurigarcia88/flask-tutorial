
# Flask-tutorial

This a project that follows up flask official tutorial from scratch.
Users are able to register, log in, create posts, and edit or delete their own posts by using a sql databse

## Project layout
```
/<your_project_path>/flask-tutorial
├── flaskr/
│   ├── __init__.py
│   ├── db.py
│   ├── schema.sql
│   ├── auth.py
│   ├── blog.py
│   ├── templates/
│   │   ├── base.html
│   │   ├── auth/
│   │   │   ├── login.html
│   │   │   └── register.html
│   │   └── blog/
│   │       ├── create.html
│   │       ├── index.html
│   │       └── update.html
│   └── static/
│       └── style.css
├── tests/
│   ├── conftest.py
│   ├── data.sql
│   ├── test_factory.py
│   ├── test_db.py
│   ├── test_auth.py
│   └── test_blog.py
├── venv/
├── setup.py
└── MANIFEST.in

```
## Installation 
### Install git, python, and python-venv

```
sudo apt install git
sudo apt install python3-pip
sudo apt-get install python3-venv

```

### Download repo from GitHub
```
mkdir try_app && cd try_app
git clone https://https://github.com/maurigarcia88/flask-tutorial
cd flask-tutorial
```

### Create python virtual environment and install dependencies
```
python3 -m venv venv
source venv/bin/activate
python setup.py install
```

## Run application 
```
export FLASK_APP=flaskr
export FLASK_ENV=development
flask run

```

## Testing
We’ll use pytest and coverage to test and measure the code
```
pip install pytest coverage
```

To run the tests, use the pytest command

```
pytest
```
To measure and check coverage
```
coverage run -m pytest
coverage report
coverage html
```
Open ```htmlcov/index.html```
