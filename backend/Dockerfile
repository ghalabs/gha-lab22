FROM node:20-slim
WORKDIR /app
COPY backend/package*.json ./
RUN npm install --only=production
RUN mkdir -p /app/logs && chown -R node:node /app
COPY --chown=node:node backend/ .
USER node
CMD ["npm", "start"]