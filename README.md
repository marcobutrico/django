# Step-by-step primeiros passos Django
Reference docs https://pypi.org/project/Django/
https://saralgyaan.com/posts/best-way-to-start-a-django-project-with-github-integration/


Criar a pasta do projeto
mkdir mysite
cd mysite



No terminal Git Bash

Criando e ativando o Virtual Environment
- python -m venv venv (virtualenv .)
$ virtualenv -p python3 .
# or
$ virtualenv .

# Activate on MACOS/Linux
$ source bin/activate

# Activate on Windows
.\Scripts\activate

Se precisar fazer o upgrade do pip
python.exe -m pip install --upgrade pip

$ mkdir newproject && cd newproject

Instalando o Django
- pip install django

Criar projeto
- django-admin startproject mysite

Rodar o servidor
- python manage.py runserver

Criar o .gitignore
(arquivo na pasta do projeto)

Instalar o Decouple
pip install python-decouple

Create a .env file inside the directory where manage.py file is (i.e. src)
nano .env

Open the file and copy the SECRET_KEY from your settings.py
SECRET_KEY=YOUR_SECRET_KEY

Add the following two lines in your settings.py
from decouple import config
SECRET_KEY = config('SECRET_KEY')

Verifica status do git
git status

git config --global user.name "Your Real Name"
git config --global user.email "email@email.com"

git add .
git commit -m "Initial Commit"


git push -u origin main

git status

git remote add origin https://github.com/YOUR_USER_NAME/newproject.git

