FROM debian
ENV TS3SERVER_LICENSE="accept"
EXPOSE 9987/udp 10011 30033
RUN apt-get update && apt-get install -y wget && apt-get install -y bzip2
RUN wget -O /teamspeak.tar.bz2 http://dl.4players.de/ts/releases/3.2.0/teamspeak3-server_linux_amd64-3.2.0.tar.bz2
RUN ls
RUN tar -xjvf teamspeak.tar.bz2
WORKDIR teamspeak3-server_linux_amd64
CMD ./ts3server_minimal_runscript.sh
