FROM node:21

# Set up the working directory
WORKDIR /app

# Copy package.json and package-lock.json for npm install
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the application files
COPY . .

# Copy .env file if needed
COPY .env.sample .env

# Expose the port your app runs on
EXPOSE 5000

# Start the app
CMD ["npm", "start"]
