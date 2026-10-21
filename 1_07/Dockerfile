FROM ubuntu:24.04

WORKDIR /usr/src/app

COPY script.sh .

RUN chmod +x script.sh

RUN apt-get update -y

RUN apt-get install curl -y

CMD ["./script.sh"]