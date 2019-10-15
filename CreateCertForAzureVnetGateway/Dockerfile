FROM ubuntu:latest

RUN apt-get update

RUN apt-get install strongswan strongswan-pki libstrongswan-extra-plugins curl openssh-client -y

RUN curl -sL https://aka.ms/InstallAzureCLIDeb | bash

WORKDIR /tmp

COPY createCert.sh createCert.sh

# RUN ipsec pki --gen --outform pem > caKey.pem

# RUN ipsec pki --self --in caKey.pem --dn "CN=VPN CA" --ca --outform pem > caCert.pem

# RUN openssl x509 -in caCert.pem -outform der | base64 -w0 ; echo

# RUN export PASSWORD="password"
# RUN export USERNAME="client"

# RUN ipsec pki --gen --outform pem > "${USERNAME}Key.pem"
# RUN ipsec pki --pub --in "${USERNAME}Key.pem" | ipsec pki --issue --cacert caCert.pem --cakey caKey.pem --dn "CN=${USERNAME}" --san "${USERNAME}" --flag clientAuth --outform pem > "${USERNAME}Cert.pem"

# RUN openssl pkcs12 -in "${USERNAME}Cert.pem" -inkey "${USERNAME}Key.pem" -certfile caCert.pem -export -out "${USERNAME}.p12" -password "pass:${PASSWORD}"

