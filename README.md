# Диплом

## Перечень программ для дипломного проекта:
* Docker Desktop - Приложение для скачивания и установки контейнеров (в нашем случае понадобится для установки 
и использования БД(MySQL и PostgeSQL) и эмулятора банковского сервиса написанного на NodeJS).
* IntelliJ IDEA - Среда разработки и запуска програм написанных на различных языках.
* Git - Cистема управления версиями с распределенной архитектурой. Нужна для отслеживания и ведения истории 
и изменения файлов в проекте.

### Необходимо для начала работы:
1. Скачать репозиторий на локальную машину. (https://github.com/DanilaEvteev/Diplom.git).
2. Запустить Docker Decktop.
3. Запустить IntelliJ IDEA.
4. Открыть проект в IntelliJ IDEA.

### mySQL:
1. Запустить Docker c локальной машины;
2. Открыть окно терминала и в командной строке набрать команду:
   docker-compose up -d
3. В IntelijIDEA в терминале набрать docker-compose up --build;
4. В терминале запустить jar файл (командой java -jar <Наименование фала .jar>, автоматически должен запуститься СП на порту 9999);
5. Открыть новую вкладку в терминале и запустить тесты ./gradlew clean test "-Ddb.url=jdbc:mysql://localhost:<исползуемый порт>/<Наименование бд>";

### PostgreSQL:
1. Запустить Docker с локальной машшины;
2. Открыть окно терминала и в командной строке набрать команду:
   docker-compose up -d
3. В IntelijIDEA в терминале набрать docker-compose up --build;
4. В терминале запустить jar файл (командой java -jar <Наименование фала .jar>, автоматически должен запуститься СП на порту 9999);
5. Открыть новую вкладку в терминале и запустить тесты ./gradlew clean test "-Ddb.url=jdbc:mysql://localhost:<исползуемый порт>/<Наименование бд>";

## Документация:

[Задание](https://github.com/netology-code/qa-diploma)
