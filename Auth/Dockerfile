FROM node:14
WORKDIR /usr/src/app

COPY package*.json ./

# Install dependencies
RUN npm install

COPY . .

# Expose the port the app runs on
EXPOSE 3226

# Command to run the app
CMD ["npm", "start"]