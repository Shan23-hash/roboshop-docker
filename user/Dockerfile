FROM node:20

# Set working directory
WORKDIR /opt/server

# Copy everything in the current context (including .js, folders, etc.)
COPY . .

# Install dependencies
RUN npm install

# Set environment variables
ENV MONGO="true" \
    REDIS_URL="redis://redis:6379" \
    MONGO_URL="mongodb://mongodb:27017/users"

# Start the app
CMD ["node", "server.js"]
