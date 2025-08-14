# # Use Node.js LTS as base image
# FROM node:20-alpine

# # Set working directory
# WORKDIR /usr/src/app

# # Copy package.json and package-lock.json
# COPY package*.json ./

# # Install dependencies
# RUN npm install

# # Copy the rest of the backend code
# COPY . .

# # Expose port your backend runs on
# EXPOSE 5000

# # Start the backend
# CMD ["node", "app.js"]



# Use Python 3.12 Alpine as base image
FROM python:3.12-alpine

# Set working directory
WORKDIR /usr/src/app

# Copy requirements.txt and install dependencies
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the backend code
COPY . .

# Expose the port your backend runs on
EXPOSE 5000

# Start the backend
CMD ["python", "app.py"]
