команда для запуска: ansible-playbook -i inventory/prod.yml site.yml --ask-become-pass

--ask-become-pass необходим тк в процессе создается директория в opt


play для java:
  1. загрузка архива
  2. создание директории 
  3. разархивирование пакета в директорию
  4. экспорт переменных окружения (Java_home, PATH)
play для elasticsearch:
  1.
