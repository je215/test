# Use an official Node.js runtime as a parent image
FROM node:14-alpine

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json to the working directory
COPY package*.json ./

#RUN npm install cors \
#    && npm install -g nodemon 

RUN npm install -g

# Copy the rest of your application code to the working directory
COPY . .

EXPOSE 3000

# Command to start your Node.js application
CMD ["npm", "start"]