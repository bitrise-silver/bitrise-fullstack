# Use the official Node image to create a binary.
# https://hub.docker.com/_/node
FROM node:20-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json files to the container
COPY package*.json ./

# Install project dependencies
RUN npm install

# Copy the rest of the application code to the container
COPY . .

# Specify the command to start the React app
CMD ["npm", "start"]