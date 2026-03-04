FROM node:18
WORKDIR /app
# This copies the package.json from the same folder as the Dockerfile
COPY package*.json ./ 
RUN npm install
# This copies everything else (including the src folder)
COPY . . 
CMD ["node", "src/index.js"]
