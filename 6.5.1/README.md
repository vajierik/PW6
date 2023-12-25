# Запуск playbook

## Запуск create_user_playbook.yml

ansible-playbook create_user_playbook.yml -vvv --ask-become-pass --ask-vault-pass


## Запуск postfix_playbook.yml
Для установки postfix

ansible-playbook postfix_playbook.yml -vvv --tags "init postfix"

Для удаления postfix

ansible-playbook postfix_playbook.yml -vvv --tags "drop postfix"

