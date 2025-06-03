# Production Dockerfile for Node.js Backend

FROM node:20.11.0

WORKDIR /app

COPY package.json package-lock.json ./
RUN npm install --production

COPY . ./

EXPOSE 5000

CMD ["node", "index.js"] # Adjust if your main file is app.js or server.js
