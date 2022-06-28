FROM node:14-alpine

#here we're defining the working directory
WORKDIR /usr/src/app

# copy app dependencies
COPY package*.json ./

# install dependencies
RUN npm install 

# copy files from app to the container
COPY . .

# expose this port to access the container
EXPOSE 3000

# starting the application
CMD ["npm", "run", "start"]