FROM node:20-slim
RUN apt-get install -y git
WORKDIR /app
COPY backend/package*.json ./
RUN npm install --only=production
COPY backend/ .
CMD ["node", "src/app.js"]