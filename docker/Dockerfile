FROM phpdockerio/php:8.4-cli

LABEL org.opencontainers.image.authors="samuele.lilli@gmail.com"

COPY --from=composer:latest /usr/bin/composer /usr/local/bin/composer
RUN chown ubuntu:ubuntu /usr/local/bin/composer

ENTRYPOINT ["/bin/bash"]

USER ubuntu