FROM node:22

WORKDIR /app

COPY package*.json ./
RUN npm install

COPY . .

EXPOSE 3000

# 👇 optional (safe fallback)
ENV PORT=3000

CMD ["npm", "start"]