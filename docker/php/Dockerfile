FROM php:8.4-fpm-alpine

# Установка системных зависимостей
RUN apk update && apk add --no-cache \
    git \
    curl \
    libpng-dev \
    libxml2-dev \
    zip \
    unzip \
    oniguruma-dev \
    freetype-dev \
    libjpeg-turbo-dev \
    libpng-dev \
    libzip-dev \
    icu-dev \
    autoconf \
    g++ \
    make

# Установка расширений PHP с правильными зависимостями
RUN docker-php-ext-configure gd --with-freetype --with-jpeg
RUN docker-php-ext-configure intl

RUN docker-php-ext-install \
    pdo_mysql \
    mbstring \
    exif \
    pcntl \
    bcmath \
    gd \
    zip \
    intl \
    xml

# Установка Composer
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# Создание пользователя для приложения
RUN addgroup -g 1000 app && adduser -u 1000 -G app -s /bin/sh -D app

# Рабочая директория
WORKDIR /var/www/html

# Смена владельца файлов
RUN chown -R app:app /var/www/html

USER app

EXPOSE 9000

CMD ["php-fpm"]
