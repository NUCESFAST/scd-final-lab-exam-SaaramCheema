# Use an official Node.js runtime as a parent image
FROM node:14

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3226

CMD ["npm", "start"]
