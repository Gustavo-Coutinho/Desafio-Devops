FROM python:3.7-slim-buster
WORKDIR /runtime-app
COPY . .
RUN pip install -r requirements.txt
ENTRYPOINT python manage.py runserver 0.0.0.0:8000