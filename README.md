# C4 Modelling Design Wizard

## Initial Setup and Configuration (pre-coding)
python3 -m venv .venv
pip3 install pip --upgrade
pip3 install Flask
pip3 install Flask-User==1.0.2.2
pip3 install flask-mongoengine
pip3 install flask-debugtoolbar
pip3 install python-dotenv
pip3 install dnspython
pip3 install gunicorn
/Applications/Python\ 3.10/Install\ Certificates.command
pip3 install certifi
pip3 install flask-mongo-sessions
pip3 install requests

## Environment Setup
.env file with all environment variables for the local environment

## CD/CI Pipeline on GitHub and Heroku
### Local Environment Preparation
.slugignore to ensure the documentation folder isn't uploaded to Heroku.
Procfile to run gunicorn as web server on Heroku.
pip3 freeze > requirements.txt