FROM node:16.13.2

MAINTAINER yusungkim@me.com

RUN mkdir -p /usr/src/app
WORKDIR /usr/src/app

COPY ./app/package.json .
COPY ./app/yarn.lock .
RUN yarn

COPY ./app/. .

EXPOSE 3000

CMD ["yarn", "run", "start"]
