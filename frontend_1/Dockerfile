# Use Node base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Copy package.json first
COPY package.json ./

# Install dependencies
RUN npm install

# Copy rest of the code
COPY . .

# Expose port
EXPOSE 3000

# Start app
CMD ["npm", "start"]
