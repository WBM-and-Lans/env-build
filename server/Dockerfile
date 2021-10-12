FROM python:3.7-alpine
MAINTAINER WenBiming

ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

RUN mkdir /server
WORKDIR /server
COPY . /server/



RUN adduser -D user
USER user