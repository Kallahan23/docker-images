# Alpine nodejs web server with nginx reverse proxy
# Author: Danny K
#
# Usage (process):     docker run -d -v $(pwd)/server/:/usr/share/nginx/html/ -p 8080:3000 kallahan23/nginx-node
# Usage (interactive): docker run -it -v $(pwd)/server/:/usr/share/nginx/html/ -p 8080:3000 kallahan23/nginx-node

FROM nginx:alpine

# Install system deps
RUN apk -v --update add \
    build-base \
    ca-certificates \
    curl \
    libffi-dev \
    musl-dev \
    ncurses \
    nodejs \
    nodejs-npm \
    openssh-client \
    openssl-dev

# Set web root as working directory
WORKDIR /usr/share/nginx/html

## Copy default nginx config
COPY nginx.conf /etc/nginx/conf.d/default.conf
# RUN rm -rf /usr/share/nginx/html/*

# Make ports available to the world outside this container
EXPOSE 80

# Run nodejs when the container launches
CMD [ "npm", "start" ]
