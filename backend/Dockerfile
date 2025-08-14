# Use Node.js LTS as base image
FROM node:20-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the backend code
COPY . .

# Expose port your backend runs on
EXPOSE 5000

# Start the backend
CMD ["node", "app.js"]
