FROM node:14

WORKDIR /web

# Copies package.json and package-lock.json to Docker environment
COPY . .

# Installs all node packages
RUN apt install && npm install && npm install -g serve && npm run build

# Uses port which is used by the actual application
EXPOSE 5000

# Finally runs the application
CMD ["npm", "install", "&&", "npm", "start" ]

