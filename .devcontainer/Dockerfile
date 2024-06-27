# Use the official PHP image based on Alpine
FROM php:8.3-fpm-alpine
RUN set -ex && apk --no-cache add sudo
# Install Nginx, necessary PHP extensions, and tools
RUN apk update && apk add --no-cache \
    nginx \
    supervisor \
    git \
    unzip \
    curl \
    icu-dev \
    mariadb-client \
    postgresql-dev \
    libzip-dev \
    && docker-php-ext-install intl pdo pdo_mysql zip

# Install Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# Install Symfony CLI
RUN curl -1sLf 'https://dl.cloudsmith.io/public/symfony/stable/setup.alpine.sh' | sh \
    && apk add symfony-cli

# Configure Nginx
COPY ./.devcontainer/nginx.conf /etc/nginx/nginx.conf

# Configure Supervisor
COPY ./.devcontainer/supervisord.conf /etc/supervisord.conf

# Create a new user with a shell
RUN adduser -D -s /bin/sh symfony

WORKDIR /var/www/html

# Set permissions
RUN chown -R symfony:www-data /var/www/html
# Set the working directory

# Set the new user
USER symfony

# Copy current directory to working directory
COPY . /var/www/html



# Expose ports
EXPOSE 80

# Start Supervisor
CMD ["/usr/bin/supervisord", "-c", "/etc/supervisord.conf"]
