FROM ubuntu

RUN \
    apt-get update && apt-get -y upgrade &&\
    apt-get -y install curl wget zip &&\
    wget -O terraform.zip https://releases.hashicorp.com/terraform/0.13.5/terraform_0.13.5_linux_amd64.zip &&\
    unzip terraform.zip &&\
    mv terraform /usr/bin/

RUN curl -sL https://aka.ms/InstallAzureCLIDeb | bash


