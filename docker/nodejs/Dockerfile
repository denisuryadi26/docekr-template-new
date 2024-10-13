# Gunakan versi Node.js terbaru sebagai base image
FROM node:current

# Set working directory
WORKDIR /usr/src/app

# Salin file package.json dan package-lock.json
COPY public/nodejs/package*.json ./

# Install dependencies
RUN npm install

# Salin seluruh kode aplikasi ke dalam container
COPY public/nodejs/. .

# Expose port untuk aplikasi
EXPOSE 3000
ARG DOCKER_ENV
ENV NODE_ENV=dev

# Jalankan aplikasi Node.js
CMD ["npm", "start"]
