# Use an official Node.js runtime as a parent image
FROM node:18-alpine

# Set working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json before installing dependencies
COPY package.json package-lock.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Expose backend port
EXPOSE 5000

# Start the application
CMD ["npm", "start"]
