FROM node:18

WORKDIR /usr/src/app

# Install mongo client tools
RUN apt-get update \
    && apt-get install -y mongo-tools \
    && rm -rf /var/lib/apt/lists/*

COPY package*.json ./
RUN npm install
COPY . .

CMD ["node", "index.js"]
