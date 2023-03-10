#Build from nginx:alpine
FROM nginx:alpine

# Install git
RUN apk add --no-cache git

# Clear html folder
RUN rm -rf /usr/share/nginx/html/*

# Clone the repo to the html folder
RUN git clone https://github.com/broekeson/broekeson.github.io.git /usr/share/nginx/html

# Expose port 80
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]