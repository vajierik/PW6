# Run nginx-php-user.yml
Для настройки адреса php-fpm при запуске playbook'а нужно аргументом задать ip
Пример:

ansible-playbook nginx-php-user.yml -vvv --ask-become-pass --extra-vars "php_ip=158.160.32.129"