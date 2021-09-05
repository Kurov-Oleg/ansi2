команда для запуска: ansible-playbook -i inventory/prod.yml site.yml --ask-become-pass

--ask-become-pass необходим тк в процессе создается директория в opt
в процессе работы play для Кибаны идет загрузка архива, создание директории, распаковка и настройка окружения с помощью переменных, описанных в templates и group_vars
