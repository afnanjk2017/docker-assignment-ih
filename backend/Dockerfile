# Use Node.js runtime
FROM node:22-alpine

# Author
LABEL author="afnan"

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all source files
COPY . .

# Expose backend port
EXPOSE 3001

# Start server in development mode with nodemon (if installed)
CMD ["npm", "run", "dev"]

