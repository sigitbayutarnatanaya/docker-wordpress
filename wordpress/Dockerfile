# Dockerfile
FROM wordpress:5.1.1-fpm-alpine

# Install dependencies
RUN apk add --no-cache \
    curl \
    libpng-dev \
    libzip-dev \
    zip \
    unzip \
    git \
    tzdata

# Install PHP extensions
RUN docker-php-ext-install \
    pdo_mysql \
    mysqli \
    zip \
    gd

# Set working directory
WORKDIR /var/www/html 

# Expose port

EXPOSE 80
