# dev stage
FROM node:19-alpine as dev

ENV NODE_ENV development

ARG REACT_APP_BASE_API
ENV REACT_APP_BASE_API $REACT_APP_BASE_API

WORKDIR /usr/src/app/

COPY package*.json ./

RUN npm i

COPY . .

EXPOSE 3000

CMD ["npm", "start"]
