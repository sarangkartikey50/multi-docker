FROM node:14-alpine

WORKDIR /app

COPY ./package.json ./
COPY ./yarn.lock ./
RUN apk add --update yarn
RUN yarn
COPY ./ ./

CMD [ "yarn", "start" ]