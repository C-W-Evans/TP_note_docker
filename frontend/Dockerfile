# Use a compatible Node.js version
FROM node:18

# Set the working directory
WORKDIR /app

# Copy package.json and package-lock.json, then install dependencies
COPY package.json ./
RUN npm install

# Install Angular CLI globally
RUN npm install -g @angular/cli

# Copy the application code
COPY . .

# Expose Angular's default port
EXPOSE 4200

# Command to run the Angular development server
CMD ["sh", "-c", "echo 'const API_URL = /api/v1;' > /src/.env && ng serve --host 0.0.0.0"]