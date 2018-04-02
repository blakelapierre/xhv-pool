FROM ubuntu

RUN apt-get update
RUN apt-get install -y wget unzip

RUN wget https://github.com/havenprotocol/haven/releases/download/v1.0.0/haven-cli-linux-x64-1.0.0.zip
RUN unzip haven-cli-linux-x64-1.0.0.zip /coin

CMD cd coin && ./havend --data-dir /daemon-data