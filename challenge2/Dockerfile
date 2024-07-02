# Start with the official Node.js image based on Alpine Linux
FROM node:alpine

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies defined in package.json
RUN npm install

# Copy the remaining application code to the container
COPY . .

# Expose port 3000 to allow connections to the application
EXPOSE 3000

# Specify the command to start the application
CMD ["node", "server.js"]

