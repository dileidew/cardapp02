FROM node:12.18.3-alpine

ENV APP_HOME /app
RUN mkdir -p $APP_HOME
WORKDIR $APP_HOME

# 第一回目の docker-compose build は下記
# RUN apk update && npm install -g @vue/cli

# 第二回目以降の docker-compose build は下記
RUN apk update
COPY package.json .
RUN npm install