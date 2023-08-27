FROM node:latest

WORKDIR /app/medusa

COPY . .

RUN apt-get update

RUN apt-get install -y python-is-python3

RUN npm install -g npm@latest   

RUN npm install --loglevel=error

ENTRYPOINT ["./develop.sh", "develop"]
    