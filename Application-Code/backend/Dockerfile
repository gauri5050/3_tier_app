FROM node:14

WORKDIR /usr/src/app

# Install Mongo CLI
RUN apt-get update && apt-get install -y mongodb-clients

COPY package*.json ./
RUN npm install
COPY . .

CMD ["node", "index.js"]
