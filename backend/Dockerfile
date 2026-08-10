FROM node:20-slim
WORKDIR /app
COPY backend/package*.json ./
RUN npm install --only=production
COPY . .
USER root
CMD ["npm", "start"]