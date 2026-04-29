FROM node:18
WORKDIR /app
COPY . .
RUN npm install
RUN npm run build

FROM nginx:alpine
COPY --from=0 /app/dist /usr/share/nginx/html