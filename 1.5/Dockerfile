FROM ubuntu:16.04

# Install tooling
RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash
RUN apt install -y nodejs

# Build app
COPY . .
RUN npm install

# Run app
EXPOSE 5000
CMD npm start
