# Nginx + php-fpm role
## При запуске playbook'а без аргументов, documet_root будет дефолтным (/var/www/html)

ansible-playbook nginx_php.yml -vvv --ask-become-pass


## Чтобы изменить document_root нужно при запуске добавить аргумент

ansible-playbook nginx_php.yml -vvv --ask-become-pass --extra-vars "document_root=/opt/nginx/ansible"

# Dnsmasq 
## Запуск осуществляется командой
ansible-playbook dnsmasq.yml -vvv --ask-become-pass

# Create super-users
## Запуск осуществляется командой
ansible-playbook create_super_users.yml -vvv --ask-become-pass
