# Gunakan image Node.js versi terbaru sebagai base image
FROM node:current

# Set working directory
WORKDIR /usr/src/app

# Salin package.json dan package-lock.json
COPY publick/reactjs/package*.json ./

# Install dependencies
RUN npm install

# Salin seluruh kode
COPY publick/reactjs/. .

# Expose port 3000
EXPOSE 3000

# Jalankan aplikasi
CMD ["npm", "start"]
