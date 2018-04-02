FROM node:0.10

RUN apt-get update && apt-get install -y git build-essential redis-server libboost1.55-all-dev nodejs-dev nodejs-legacy npm cmake libssl-dev

RUN git clone https://github.com/blakelapierre/xhv-pool

RUN cd xhv-pool/pool && npm update

EXPOSE 8117
EXPOSE 3333

ADD config.json /xhv-pool/pool/config.json

CMD cd xhv-pool/pool && node init.js