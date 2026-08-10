FROM node:20-slim
RUN apt-get update && apt-get install -y --no-install-recommends git=1:2.29.* && rm -rf /var/lib/apt/lists/*
WORKDIR /app
COPY backend/package*.json ./
RUN npm install --only=production
COPY backend/ .
CMD ["node", "src/app.js"]