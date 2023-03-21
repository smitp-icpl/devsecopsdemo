
# This Dockerfile uses the official Python image as the base image, sets the working directory in the container to `/app`, copies the application code into the container, installs the dependencies using pip, exposes port 5000, and starts the application by running the `app.py` file using the `python` command.

# ### React Application Dockerfile
# Here's a sample Dockerfile for your React application:

# ```dockerfile
# # Use the official Node.js image as the base image
# FROM node:14-alpine

# # Set the working directory in the container
# WORKDIR /app

# # Copy the application code into the container
# COPY . .

# # Install the dependencies for the application
# RUN npm install --production

# # Build the React application
# RUN npm run build

# # Expose the port that the application listens on
# EXPOSE 3000

# # Start the application
# CMD ["npm", "start"]


# ==========================

FROM node:14-alpine
WORKDIR /app
COPY package*.json ./
RUN npm install
COPY . .
CMD [ "npm", "start" ]