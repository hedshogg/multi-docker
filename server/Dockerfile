FROM node:alpine

WORKDIR "/app"

COPY ./package.json ./

RUN npm install

COPY . .

# Note this is the only change from Dockerfile.dev "dev" -> "start"
CMD ["npm", "run", "start"]