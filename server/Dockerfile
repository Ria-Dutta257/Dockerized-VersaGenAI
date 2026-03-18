# Use Node 22 image
FROM node:22

# Create working directory
WORKDIR /app

# Copy package files first
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy remaining server code
COPY . .

# Expose backend port
EXPOSE 3000

# Start server
CMD ["npm","run","server"]