# www.youtube.com/watch?v=MbA71IuYUhg solution
FROM node:18.14.1 as angular
LABEL authors="ttknpde-v"

WORKDIR /usr/src/app

# remember (.) dot it means goto WORKDIR AS /usr/src/app
# it's very importance
# COPY package.json .
# COPY package-lock.json .
# can reduce lines
COPY package.json package-lock.json /usr/src/app/

RUN npm install

# first (.) means Where I am now
COPY . /usr/src/app

EXPOSE 4200

# command run utill has interupt
# it means that it can be accessed via all the IP addresses on all interfaces on the machine, including 127.0. 0.1
CMD /usr/src/app/node_modules/.bin/ng serve --host 0.0.0.0
