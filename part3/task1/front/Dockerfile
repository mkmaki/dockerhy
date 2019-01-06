FROM ubuntu:16.04

RUN apt-get update && apt-get install -y git nodejs npm && \
  git clone https://github.com/docker-hy/frontend-example-docker.git /app && \
  npm install && \
  apt-get purge -y --auto-remove git && \
  rm -rf /var/lib/apt/lists/*
EXPOSE 5000

WORKDIR /app

CMD API_URL=http://localhost:8000 npm start
