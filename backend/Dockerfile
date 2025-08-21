# Use Node base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Copy package.json first (for caching layers)
COPY package.json ./

# Install dependencies
RUN npm install

# Copy rest of the code
COPY . .

# Expose port
EXPOSE 5000

# Start app
CMD ["npm", "start"]
