FROM node:8-slim

RUN apt-get update
RUN apt-get install -y git
RUN git clone https://github.com/socketio/socket.io.git
WORKDIR socket.io
RUN npm install
WORKDIR examples/chat
RUN npm install
