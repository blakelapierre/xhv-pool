FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget unzip

RUN wget https://github.com/havenprotocol/haven/releases/download/v1.0.0/haven-cli-linux-x64-1.0.0.zip
RUN unzip -j haven-cli-linux-x64-1.0.0.zip -d /coin

CMD cd coin && ./havend --data-dir /daemon-data