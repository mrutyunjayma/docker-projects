# official image of the node
FROM node:18.9.1

#set working directory
WORKDIR /app

# copy the package.json file to the container
COPY package.json* ./

RUN npm install

COPY . .

EXPOSE 5050

CMD ["npm", "start"]