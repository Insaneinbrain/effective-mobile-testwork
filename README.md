## Description
Данный набор скриптов содержит плейбук с двумя ролями:
- Роль **docker** устанавливает Docker и Docker-compose.
- Роль **app** копирует конфигурационные файлы веб-приложения и запускает его в контейнерах.

В ```inventory.yaml``` изменить IP-адрес настраиваемого сервера, после настраивается к нему доступ по ssh-ключу, далее запуск конфигурирования осуществляется командой ```ansible-playbook playbook.yaml -i inventory.yaml```.

Набор скриптов адаптирован для дистрибутива Ubuntu 22.04.

После запуска приложение будет доступно по адресу http://IP-сервера/