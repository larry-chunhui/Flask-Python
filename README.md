########################
# create the website ref the video:
https://www.youtube.com/watch?v=Z1RJmh_OqeA
########################
https://flaskchunhui.herokuapp.com/

########################
installation process:
########################
virtualenv --python=/usr/bin/python3.7 env
source env/bin/activate
python3.7 -m pip install flask flask-sqlalchemy


heroku login
touch Procfile
python3.7 -m pip install gunicorn
python3.7 -m pip  freeze > requirements.txt
git init
git add .
git commit -m "initial app"

heroku create flaskchunhui
heroku git remote -v

git push heroku master
