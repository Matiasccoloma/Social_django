FROM alpine:3.18
RUN apk upgrade --no-cache
RUN apk add python3
RUN apk add py3-pip
COPY ./social_django /opt/app/social_django

WORKDIR /opt/app/social_django
RUN pip install -r requirements.txt

CMD python3 manage.py runserver 0.0.0.0:9000