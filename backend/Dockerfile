FROM node:12.19.0-alpine

# Create app directory
WORKDIR /usr/app/

# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY ./package*.json ./

# If you are building your code for production
# RUN npm ci --only=production
#RUN npm ci -qy
RUN npm install

# Bundle app source
COPY backend/ ./backend

# Expose Port 3000
EXPOSE 3000

CMD ["npm", "run", "dev"]