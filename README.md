# SMS

https://up.algomojo.com/xl-connect/am/login-response?id=3UAN9Y

http://127.0.0.1:8000

https://option-339618.el.r.appspot.com

http://15.206.54.144:8000/

pip install virtualenv
python -m virtualenv env
env\Scripts\activate
python manage.py runserver
python runserver.py
python manage.py runserver 0.0.0.0:8000
pip freeze > requirements.txt
pip install -r requirements.txt
python -m pip install --upgrade pip

gcloud app create
gcloud config set project option-339618
gcloud auth application-default login

gcloud auth login
cloud_sql_proxy -instances=option-339618:asia-south1:option=tcp:3306

python manage.py makemigrations
python manage.py makemigrations polls
python manage.py migrate
python manage.py collectstatic

python manage.py runserver
python manage.py runserver 0.0.0.0:8000
python manage.py createsuperuser

gcloud app deploy
gcloud app logs tail -s default
gcloud app browse
gcloud components update

#################pip install ##########

pip install gunicorn

gunicorn --bind 0.0.0.0:8000 Main.wsgi
