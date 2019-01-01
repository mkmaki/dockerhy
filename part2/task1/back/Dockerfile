FROM ubuntu
WORKDIR /mydir

RUN apt-get update && apt-get install -y git nodejs npm
RUN git clone https://github.com/docker-hy/backend-example-docker.git /mydir
RUN npm install
EXPOSE 8000

CMD FRONT_URL=http://localhost:5000 npm start
