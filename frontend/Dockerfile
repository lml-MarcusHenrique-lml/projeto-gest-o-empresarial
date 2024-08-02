# Dockerfile para o frontend React
FROM node:18

WORKDIR /usr/src/app

COPY package*.json ./
RUN npm install

COPY . .

RUN npm run build

# Servir a aplicação com um servidor estático
RUN npm install -g serve
CMD ["serve", "-s", "build"]

EXPOSE 3000
