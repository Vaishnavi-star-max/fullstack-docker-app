# Use Node.js base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Copy package.json and install dependencies
COPY package*.json ./
RUN npm install

# Copy all files into the container
COPY . .

# Expose frontend port
EXPOSE 3000

# Start the React development server
CMD ["npm", "start"]
