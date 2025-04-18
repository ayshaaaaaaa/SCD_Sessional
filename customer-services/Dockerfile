# Use Node.js image
FROM node:18

# Set working directory
WORKDIR /app

# Copy package files and install dependencies
COPY package*.json ./
RUN npm install

# Copy the rest of the app
COPY . .

# Expose the port
EXPOSE 3002

ENV NODE_ENV=production

# Run the service
CMD ["node", "index.js"]
