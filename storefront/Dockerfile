FROM node:latest

WORKDIR /app/storefront

COPY . .

RUN apt-get update

RUN npm install -g npm@latest

RUN npm install --loglevel=error

RUN npm run build

ENTRYPOINT ["npm", "run", "start" ]