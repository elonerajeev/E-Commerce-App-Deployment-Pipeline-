# Production Dockerfile for React Frontend

FROM node:20.11.0 AS builder

WORKDIR /app

COPY package.json package-lock.json ./
RUN npm install

COPY . ./
RUN npm run build

# Serve the static build using nginx
FROM nginx:stable-alpine

COPY --from=builder /app/build /usr/share/nginx/html

# Copy custom nginx config if needed
# COPY nginx.conf /etc/nginx/nginx.conf

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
