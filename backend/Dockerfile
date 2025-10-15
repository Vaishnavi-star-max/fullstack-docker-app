# Use Node.js base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the backend code
COPY . .

# Expose backend port
EXPOSE 5000

# Start the server
CMD ["npm", "start"]
