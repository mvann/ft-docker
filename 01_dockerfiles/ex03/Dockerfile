FROM ubuntu:14.04

RUN apt-get update &&\
	apt-get install -y \
	git\
	curl
RUN curl https://cdn.gogs.io/0.11.53/gogs_0.11.53_linux_amd64.tar.gz -o gogs.tar.gz
RUN tar -xzf gogs.tar.gz
WORKDIR /gogs
CMD ./gogs web
