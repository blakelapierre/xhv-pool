FROM ubuntu:14.04

RUN apt-get update && apt-get install -y git build-essential redis-server libboost1.55-all-dev nodejs-dev nodejs-legacy npm cmake libssl-dev

RUN git clone https://github.com/blakelapierre/etn-pool

RUN cd etn-pool/pool && npm update

EXPOSE 8117
EXPOSE 3333

ADD config.json /etn-pool/pool/config.json

CMD cd etn-pool/pool && node init.js