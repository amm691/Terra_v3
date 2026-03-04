FROM node:18

WORKDIR /app

# Copy dependency files
COPY package*.json ./
RUN npm install

# Copy the rest of the code (including the src folder)
COPY . .

# Match the port to your Service YAML (TargetPort)
EXPOSE 8080 

# FIX: Added 'src/' to the path
CMD ["node", "src/index.js"]
