Цель дз развернуть InnoDB кластер 

Для этого Запускаем три ноды для InnoDB Cluster с помощью vagrant

Ansible ставит mysql-server и mysql-shell

Для создания машин запускаем команду:
vagrant up

далее, для установки mysql server и шел выполнить следующие команды:
cd provision

ansible-playbook playbooks/environment.yml

проверить корректность установки ключа для логина по ssh можно командой:

vagrant ssh mysql1

vagrant ssh mysql2

vagrant ssh mysql3
