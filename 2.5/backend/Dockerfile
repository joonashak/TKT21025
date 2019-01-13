FROM ubuntu:16.04

# Install tooling
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs

# Build app
COPY . .
RUN npm install

# Run app
EXPOSE 8000
CMD FRONT_URL=http://localhost:5000 npm start