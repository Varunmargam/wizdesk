# Use the official Node.js base image
FROM node:16-alpine

# Set the working directory inside the container
WORKDIR /app

# Copy the package.json and package-lock.json files into the container
COPY package*.json ./

# Install the dependencies
RUN npm install

# Copy the application code into the container
COPY . .

# Expose the port that the application runs on
EXPOSE 3002

# Start the application
CMD ["node", "server.js"]
