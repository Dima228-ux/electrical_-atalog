# electrical_catalog

## Backend

1.  Переходим в директорию

        cd source-code

2.  Копируем .env.example в .env

3.  Скачиваем зависимости

        composer install

4.  Создаем базу данных

        CREATE USER "electrical-catalog" WITH PASSWORD '12345';
        CREATE DATABASE "electrical-catalog" WITH OWNER 'electrical-catalog';

5.  Запускаем миграции базы данных:

        php artisan migrate

6.  Запускаем сидеры:

        php artisan db:seed

7.  Генерируем ключ приложения:

        php artisan key:generate

8.  Запускаем сервер

        php artisan serve
