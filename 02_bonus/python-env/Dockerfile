FROM debian

RUN apt-get update &&\
	apt-get -y upgrade &&\
	apt-get install -y \
	python-pip
RUN pip install jupyter
EXPOSE 8888
ENTRYPOINT jupyter notebook --ip=0.0.0.0 --allow-root
