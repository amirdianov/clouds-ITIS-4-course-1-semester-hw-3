### Настройка проекта

Для корректного запуска проекта требуется:

1. Изменить путь к ssh ключу файла `main.tf`
2. Заменить IP в файле `hosts` на результат работы команды `terraform apply`
3. Заменить PATH в файле `hosts` на путь к ssh ключу
4. Выполнить команду `ansible-playbook --become --become-user root --become-method sudo -i hosts nextcloud.yaml`