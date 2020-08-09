FROM    ichikawayukko/php-fpm_pgsql

RUN     cd /tmp && \
        php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
        php composer-setup.php && \
        php -r "unlink('composer-setup.php');" && \
        mv composer.phar /usr/local/bin/composer && \
        chmod +x /usr/local/bin/composer && \
        apk add npm
