FROM node:10

# Create app directory
WORKDIR /usr/src/lafs

# Install app dependencies
# A wildcard is used to ensure both package.json and package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./

RUN npm install
# If code is for production
# RUN npm ci --only=production

# Bundle app source
COPY . .

# Expose port 3000
EXPOSE 3000

CMD npm run start