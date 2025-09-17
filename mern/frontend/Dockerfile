# official image of node
FROM node:18.9.1

# Set the directory of project
WORKDIR /app

#copy the package json file to the work directory
COPY package.json* ./

# install npm to the container
RUN npm install


#EXPOSE the port for inform the docker is running on this port
EXPOSE 5173

# Copy the all source file to the  from the host to app
COPY . .

# Run the specified command within the container
CMD ["npm", "run", "dev"]