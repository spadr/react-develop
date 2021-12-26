FROM node:17-alpine

WORKDIR /usr/src/app

RUN npm install -g npm

RUN npm install --save typescript react-apexcharts apexcharts

RUN npm install --save-dev \
    eslint prettier \
    eslint-config-prettier @typescript-eslint/eslint-plugin @typescript-eslint/parser \
    eslint-config-prettier eslint-plugin-react eslint-plugin-react-hooks\
    jest @types/jest ts-jest

COPY . .