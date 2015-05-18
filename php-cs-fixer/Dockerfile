# php-cs-fixer Docker Container
FROM composer/composer
MAINTAINER Ludovic Fleury <ludo.fleury@gmail.com>

# Goto temporary directory
WORKDIR /tmp

# Run composer and php-cs-fixer installation.
RUN composer selfupdate && \
  composer require "fabpot/php-cs-fixer:*" --dev && \
  ln -s /tmp/vendor/bin/php-cs-fixer /usr/local/bin/php-cs-fixer

# Set up the application directory.
VOLUME ["/app"]
WORKDIR /app

# Set up the command arguments.
ENTRYPOINT ["/usr/local/bin/php-cs-fixer"]
CMD ["--help"]
