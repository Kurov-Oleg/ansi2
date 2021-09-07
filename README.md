команда для запуска: ansible-playbook -i inventory/prod.yml site.yml --ask-become-pass

--ask-become-pass необходим тк в процессе создается директория в opt


play для java:
  1. поиск архива в локальном хранилище
  2. создание директории (/opt/jdk/{{ java_jdk_version }})
  3. разархивирование пакета в директорию
  4. экспорт переменных окружения (Java_home, PATH)

play для elasticsearch:
  1. загрузка архива с сайта
  2. создание директории (/opt/elastic/{{ elastic_version }})
  3. разархивирование пакета
  4. экспорт переменных окружения (ES_HOME,PATH)

play для kibana:
  1. загрузка архива с сайта
  2. создание директории (/opt/kibana/{{ kibana_version }})
  3. разархивирование пакета
  4. экспорт переменных окружения (KIB_HOME,PATH)
