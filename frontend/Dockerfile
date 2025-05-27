# Use official Node.js image as base
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Install dependencies
COPY . /app
RUN npm install

# Build the frontend
RUN npm run build

# Expose port 4173 for Vite preview
EXPOSE 5173

# Start Vite preview server
CMD ["npm", "run", "dev", "--", "--host"]
