# Лабораторная работа 4 - DevOps-автоматизация

## Структура проекта
- `ansible/site.yml` — основной плейбук развертывания
- `ansible/inventories/inventory.ini` — файл инвентаря
- `ansible/scripts/` — bash-скрипты сервиса и healthcheck
- `ansible/systemd/` — systemd unit-файл службы

## Запуск Ansible
```bash
ansible-playbook -i ansible/inventories/inventory.ini ansible/site.yml -K
