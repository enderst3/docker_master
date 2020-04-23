# Use the official image as parent image.
FROM node:current-slim

#Set working directory.
WORKDIR /app

# Copy the file from your host to your current location.
COPY package.json .

# Run the command inside your image filesystem.
RUN npm install

# Inform Docker that the container is listening on the specifified port at runtime.
EXPOSE 8080

# Rind the specified command within the container.
CMD [ "npm", "start" ]

# Cope the rest of your app's source code from your host to your image filesystem.
COPY . .