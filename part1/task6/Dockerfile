#docker run -p 8000:8000 -v $(pwd)/logs.txt:/mydir/logs.txt kontti
#12/30/2018, 1:26:21 PM: Connection received in root
#12/30/2018, 1:26:22 PM: Connection received in root
#12/30/2018, 1:26:35 PM: Connection received in root

FROM ubuntu
WORKDIR /mydir

RUN apt-get update && apt-get install -y git nodejs npm
RUN git clone https://github.com/docker-hy/backend-example-docker.git /mydir
RUN npm install
EXPOSE 8000

CMD npm start
