# syntax=docker/dockerfile:1
FROM ubuntu:24.04 as base

RUN \
  apt-get update -y && \
  apt-get install -y ruby

WORKDIR /simple_server

COPY . /simple_server

ENV PORT=9292

EXPOSE 9292

RUN gem install bundler && bundle update && bundle install

CMD ["rackup", "--host", "0.0.0.0", "-p", "9292"]

