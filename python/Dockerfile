FROM python:3.7

RUN mkdir -p /app
WORKDIR /app

RUN apt update && apt upgrade -y
RUN /usr/local/bin/python -m pip install --upgrade pip
RUN /usr/local/bin/python -m pip install --upgrade setuptools

COPY requirements.txt /app
RUN pip install -r requirements.txt
