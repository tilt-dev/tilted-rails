FROM ruby:3-slim-bullseye

RUN apt-get update -y && \
    apt-get install -y build-essential git libpq-dev

RUN gem install rails --no-doc

RUN mkdir /app
WORKDIR /app

COPY . /app
