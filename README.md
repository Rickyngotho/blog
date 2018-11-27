#### ERIC blog
ericblog is a web application for adding up blogs and commenting on existing blogs.
Sept,14,2018
By eric ngotho
Description
ERIC blog is a web application blog meant for Music lovers espcially Hiphop lovers.

The blog supports comments from readers and blog writers to determine whether to delete the comments or not. Users can also delete blog posts.

After the writer has posted a new blog post, subscribers will receive an email notification with a link to the blog post.

### Set-up and Installation
Prerequiites
- Python 3.6
- Ubuntu software
Clone the Repo on my  github page https://github.com/Rickyngotho/blog.git
Run the following command on the terminal: git clone && cd Blog-IP

Install Postgres

Create a Virtual Environment
Run the following commands in the same terminal:

sudo apt-get install python3.6-venv
python3.6 -m venv virtual
source virtual/bin/activate
Install dependancies
Install dependancies that will create an environment for the app to run pip3 install -r requirements

#### Prepare environment variables
export DATABASE_URL='postgresql+psycopg2://<your-username>:<your-password>@localhost/carblog'
export SECRET_KEY='Your secret key'
export DATABASE_URL_TEST='postgresql+psycopg2://<your-username>:<your-password>@localhost/carblog_test'
export MAIL_SERVER='smtp.googlemail.com'
export MAIL_PORT=587
export MAIL_USE_TLS=1
export MAIL_USERNAME=<your-email>
export MAIL_PASSWORD=<your-password> 
Run Database Migrations
python manage.py db init
python manage.py db migrate -m "initial migration"
python manage.py db upgrade
Running the app in development
In the same terminal type: python3 manage.py server

Open the browser on http://localhost:5000/

### Known bugs
nothing yet if u ecnounter one please feel free to contact me at the email below.


### Technologies used
- Python 3.6
- HTML
- Bootstrap 4
- JavaScript
- Heroku
- Postgresql
### Support and contact details
Contact me on gicheric14@gmail.com for advice.

### License
Copyright (c) ERic NGOTHO 