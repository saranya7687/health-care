# Install Nodejs version 18 which includes npm(Node Package Manager)
FROM node:18

# Setup the working directory
WORKDIR /app

# Copy the dependencies(package.json) listed in local project to container's working directory
COPY package*.json ./

# Install the dependencies from package.json using npm
RUN npm install

# Copy all the project files
COPY . .

# Default port for application
EXPOSE 3000

# Commands to run when container starts
CMD ["npm", "start"]
