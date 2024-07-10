# Use an official PHP base image
FROM php:7.4-apache

RUN docker-php-ext-install pdo_mysql

# Set the working directory
WORKDIR /var/www/html

# Copy the PHP application code to the container
COPY . /var/www/html/

# Install any additional dependencies or tools
# For example, if using Composer for dependency management:
# RUN apt-get update && apt-get install -y composer
# RUN composer install --no-dev

# Expose the port the web server will run on
EXPOSE 80

# Define the command to start the web server
CMD ["apache2-foreground"]
