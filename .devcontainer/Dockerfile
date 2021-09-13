FROM ubuntu:20.04
LABEL Name=TheOdinProject Version=0.0.1

# Check for updates and install any
RUN apt-get -y update && apt-get install -y

# Set timezone 
ENV TZ=Europe/Copenhagen
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

# Install Git
RUN apt-get install git -y

# Install nodejs & npm
RUN apt-get install nodejs -y
RUN apt-get install npm -y

# Install TypeScript support
RUN npm install -g typescript