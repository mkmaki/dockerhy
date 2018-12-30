docker run -it curler

FROM ubuntu

WORKDIR /mydir
COPY script .
RUN apt-get update && apt-get install -y curl

CMD ./script

