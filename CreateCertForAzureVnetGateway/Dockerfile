FROM ubuntu:latest

RUN apt-get update

RUN apt-get install strongswan strongswan-pki libstrongswan-extra-plugins curl openssh-client -y

RUN curl -sL https://aka.ms/InstallAzureCLIDeb | bash

WORKDIR /tmp

COPY createCert.sh createCert.sh
