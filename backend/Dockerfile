# --- Base Image ---
FROM node:18

# --- Working Directory ---
WORKDIR /app

# --- Copy package.json and install dependencies ---
COPY package*.json ./
RUN npm install

# --- Copy all source code ---
COPY . .

# --- Expose backend port ---
EXPOSE 3000

# --- Start the backend server ---
CMD ["node", "server.js"]
