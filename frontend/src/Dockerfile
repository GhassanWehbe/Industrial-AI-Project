# Use the official Node.js image
FROM node:14

# Set the working directory inside the container
WORKDIR /app

# Copy the local code to the container image
COPY pachage-lock.json /app/
COPY src /app/

# Install dependencies
RUN npm install --from-lock-json

# Configure the environment variable needed for Node.js
ENV NODE_OPTIONS="--openssl-legacy-provider"

# Expose the port the app runs on
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
