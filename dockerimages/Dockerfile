FROM node:18-alpine AS stage
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
RUN npm build 
EXPOSE 3000
CMD [ "npm", "index.js"] 