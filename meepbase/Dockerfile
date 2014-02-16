# ubuntu 13.10 + node.js
FROM stackbrew/ubuntu:13.10

MAINTAINER meepshop "https://github.com/meepshop"

# make sure the package repository is up to date and update ubuntu
RUN echo "deb http://archive.ubuntu.com/ubuntu saucy main universe" > /etc/apt/sources.list
RUN apt-get update
RUN apt-get -y upgrade

# Install Node.js
RUN apt-get install -y software-properties-common
RUN add-apt-repository -y ppa:chris-lea/node.js
RUN apt-get update
RUN apt-get install -y nodejs

# Append to $PATH variable.
RUN echo '\n# Node.js\nexport PATH="node_modules/.bin:$PATH"' >> /root/.bash_profile


