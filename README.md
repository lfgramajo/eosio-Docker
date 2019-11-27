# eosio-Docker
:~/myimages$ cat Dockerfile 
#Download base image ubuntu 18.04
FROM ubuntu:18.04
# Update Ubuntu Software repository
RUN apt update
# Necesario para descargar
RUN apt install -y wget
# Instalar EOSIO https://github.com/EOSIO/eos
RUN wget https://github.com/eosio/eos/releases/download/v1.8.1/eosio_1.8.1-1-ubuntu-18.04_amd64.deb
#RUN sudo apt install ./eosio_1.8.1-1-ubuntu-18.04_amd64.deb
RUN apt install -y ./eosio_1.8.1-1-ubuntu-18.04_amd64.deb
