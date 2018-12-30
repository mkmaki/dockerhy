#docker run -p 8000:5000 kontti

FROM ubuntu
WORKDIR /mydir

RUN apt-get update && apt-get install -y git nodejs npm
RUN git clone https://github.com/docker-hy/frontend-example-docker.git /mydir
RUN npm install
EXPOSE 8000

CMD npm start
