# Use the official Node.js image as base
FROM node:18

# Set the working directory inside the container
WORKDIR /Teacher_STudent_API

# Copy package.json and package-lock.json (if available)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the entire project to the container
COPY . .

# Expose port 3000 for the API
EXPOSE 3001

# Run tests when the container is started
CMD ["npm", "test"]
