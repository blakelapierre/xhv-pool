FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget unzip

RUN wget https://github.com/electroneum/electroneum/releases/download/v0.11.0.0-revert/linux-x64-v0.11.0.0-revert.zip
RUN unzip linux-x64-v0.11.0.0-revert.zip -d /coin

CMD cd coin && ./electroneumd --data-dir /daemon-data