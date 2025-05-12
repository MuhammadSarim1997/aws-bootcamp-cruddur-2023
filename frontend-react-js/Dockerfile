FROM node:24.0.1

ENV PORT=3000
ENV HOST=0.0.0.0

WORKDIR /app

# Copy package.json and package-lock.json for layer caching
COPY package*.json ./

# Install dependencies (including react-scripts)
RUN npm install

# Copy the full source code
COPY . .

EXPOSE ${PORT}

CMD ["npm", "start"]
