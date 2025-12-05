FROM node:20-alpine

WORKDIR /app

# Copy package files nếu có
COPY package*.json ./

# Install dependencies nếu package.json tồn tại
RUN if [ -f package.json ]; then npm install; fi

# Copy toàn bộ code
COPY . .

# Expose port
EXPOSE 3000

# Start command
CMD ["npm", "start"]