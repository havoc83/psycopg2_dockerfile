FROM python:3.7-alpine AS build

RUN apk update \
 && apk add \
    build-base \ 
    gcc \
    libffi-dev \ 
    libpq \
    musl-dev \ 
    python3-dev \
    postgresql-dev 
    
WORKDIR /usr/src/app

RUN pip install --upgrade pip \
 && pip install psycopg2

CMD ["python"]
