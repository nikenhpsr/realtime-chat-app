# Use a base image with Node.js
FROM node:14

# Set the working directory to /app
WORKDIR /app

# Copy the backend directory into the container at /app
COPY ./backend /app

# Install dependencies using pnpm
RUN npm install -g pnpm
RUN pnpm install

# Expose the port the app runs on
EXPOSE 3000

# Command to start the application
CMD ["pnpm", "start"]
