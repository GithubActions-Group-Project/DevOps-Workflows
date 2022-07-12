FROM ubuntu:20.04

# Install wget,Powershell
RUN apt-get update && \
    apt-get install -y wget apt-transport-https software-properties-common && \     
    wget -q https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb && \
    dpkg -i packages-microsoft-prod.deb && \
    apt-get update && \
    add-apt-repository universe && \ 
    apt-get install -y powershell

#install curl, Node.js 16 and npm 8
RUN apt-get update -y && \
    apt install -y curl git && \
    curl -sL https://deb.nodesource.com/setup_16.x | bash && \
    apt-get -y update && \
    apt-get install -y nodejs && \
    curl -L https://www.npmjs.com/install.sh | sh 
