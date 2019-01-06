FROM ubuntu:16.04

RUN apt-get update && apt-get install -y git nodejs npm && \
  git clone https://github.com/docker-hy/backend-example-docker.git /app && \  
  npm install && \
  apt-get purge -y --auto-remove git && \
  rm -rf /var/lib/apt/lists/*

EXPOSE 8000
WORKDIR /app
CMD FRONT_URL=http://localhost:5000 npm start
