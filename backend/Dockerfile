FROM node:14-alpine

# Set working directory
WORKDIR /usr/app

# Install app dependencies
COPY package*.json ./


# install dependencies
RUN npm install 

# copy files from app to the container
COPY . .

# expose this port to access the container
EXPOSE 5000

# starting the application
CMD ["npm", "server", "start"]