FROM node:8.12.0
RUN mkdir -p /usr/server
WORKDIR /usr/server
COPY package*.json ./
RUN npm install --silent

COPY . .
ENV PORT=9000
EXPOSE 9000
CMD ["npm", "run", "dev"]