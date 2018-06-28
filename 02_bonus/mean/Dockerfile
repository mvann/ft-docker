FROM node:8-slim

EXPOSE 3000
RUN apt-get update
RUN apt-get install -y git
RUN git clone https://github.com/linnovate/mean.git
WORKDIR mean
RUN npm install
RUN npm run build:prod
