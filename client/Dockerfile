FROM node:16

WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Build the React app
RUN npm run build

# Serve the React app using a static server
RUN npm install -g serve
# Set the command to run the app on port 1226 as mentioned in paper
CMD ["serve", "-s", "build", "-l", "1226"]