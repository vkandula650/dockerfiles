# Use Ubuntu 20.04 as the base image
FROM ubuntu:20.04

# Update package lists and install NGINX
RUN apt-get update && apt-get install -y nginx

# Remove the default index.html file
RUN rm -rf /usr/share/nginx/html/index.html

# Copy your custom content into the NGINX HTML directory
COPY qi /usr/share/nginx/html

# Expose port 80 to allow web traffic
EXPOSE 80

# Set the command to run NGINX in the foreground
CMD ["nginx", "-g", "daemon off;"]
