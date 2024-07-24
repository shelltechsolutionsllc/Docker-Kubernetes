FROM node:14


WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

##Argument value
ARG DEFAULT_PORT = 80
##Environment variable and use of argument value
ENV PORT $DEFAULT_PORT

##Use of environment variable
EXPOSE $PORT

CMD [ "node", "server.js" ]