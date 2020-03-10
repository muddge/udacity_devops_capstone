FROM node:10

# Working Directory
WORKDIR /usr/src/app

# Install app dependencies
# Wildcard ensures both package.json and package-lock.json are copied
# where available
COPY package*.json ./
RUN npm i -g eslint
RUN npm install

#Bundle app source
COPY . .

# Expose port 3000
EXPOSE 3000

# Run app.py at container launch
CMD ["node", "./bin/www"]