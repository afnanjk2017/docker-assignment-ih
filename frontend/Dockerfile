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

# Copy frontend code
COPY . .

# Expose frontend port
EXPOSE 3000

# Start React development server
CMD ["npm", "start"]

