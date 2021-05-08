FROM node:14.16.0-alpine

ENV PROJECT_ROOTDIR /app/

WORKDIR $PROJECT_ROOTDIR

COPY package*.json $PROJECT_ROOTDIR

RUN npm install

COPY . $PROJECT_ROOTDIR

# enable to use appPort https://code.visualstudio.com/docs/remote/devcontainerjson-reference
EXPOSE 3000
ENV HOST 0.0.0.0

# CMD ["yarn", "dev"]