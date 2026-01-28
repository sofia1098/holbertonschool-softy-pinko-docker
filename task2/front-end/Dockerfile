FROM nginx:latest

# Copy front-end files
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy nginx configuration
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf
