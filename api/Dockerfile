# instruction for the image to create an image, and we will create a container from the image
FROM node
# directory where will want to place all this
WORKDIR /app
# copy the file to the main directory
COPY package*.json ./
# run the command to install the dependencies
RUN npm install
# will will copy everything from the directory (everything) to the container
COPY . .
# expose the server port
EXPOSE 4000
# the command to run the application
CMD ["npm", "start"]