FROM node:16.13.2

MAINTAINER yusungkim@me.com

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY package.json .
COPY yarn.lock .
RUN yarn

COPY . .

EXPOSE 3000

CMD ["yarn", "run", "start"]
