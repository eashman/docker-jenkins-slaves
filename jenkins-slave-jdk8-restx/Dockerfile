FROM codetroopers/jenkins-slave-jdk8-mvn

MAINTAINER Cedric Gatay "c.gatay@code-troopers.com"
ENV DEBIAN_FRONTEND noninteractive

# Install node.js from PPA
RUN add-apt-repository ppa:chris-lea/node.js
RUN apt-get update
RUN apt-get -y install nodejs ruby ruby-dev make g++
RUN gem install sass compass --no-ri --no-rdoc
# Install bower and grunt
RUN npm install -g bower grunt grunt-cli
# Install local grunt for tests
RUN npm install grunt
