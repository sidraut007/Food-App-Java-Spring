# Build the application
FROM node:18 as build

WORKDIR /app

COPY package*.json /app

RUN npm ci

COPY . /app

RUN npm run build

# Serve the application using Nginx
FROM nginx:alpine

COPY --from=build /app/build /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
