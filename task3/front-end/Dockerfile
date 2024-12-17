# Use the latest Nginx base image
FROM nginx:latest

# Copy the front-end files to the Nginx web root directory
COPY softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy the Nginx configuration file to the appropriate directory
COPY softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf

# Expose port 9000
EXPOSE 9000
