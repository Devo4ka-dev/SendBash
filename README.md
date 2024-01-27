# Описание проекта

Этот проект представляет собой простой сервис для отправки и чтения сообщений через HTTP запросы. Пользователи могут отправлять сообщения на сервер, который сохраняет их в базе данных и возвращает уникальный URL для доступа к сообщению.

[![License: Unlicense](https://img.shields.io/badge/license-Unlicense-blue.svg)](http://unlicense.org/)

## Настройка

Для начала работы с проектом выполните следующие шаги:

1. Клонируйте репозиторий на свой локальный компьютер или сервер.
2. Установите необходимые зависимости, если таковые имеются.
3. Настройте файл `config.php` с параметрами вашей базы данных.
4. Запустите сервер и убедитесь, что все работает корректно.

## Настройка базы данных

Для создания необходимой структуры базы данных, выполните следующий SQL запрос:

```sql
CREATE TABLE messages (
    id INT AUTO_INCREMENT PRIMARY KEY,
    message TEXT NOT NULL,
    random_id VARCHAR(7) NOT NULL UNIQUE
);

## требование

1. PHP 7.4 или выше.
2. Веб сервер Nginx/Apache или другой.


## Пример использования
Чтобы отправить и записать сообщение, выполните следующую команду в консоли:

echo "ваше сообщение" | curl -X POST -d @- https://kmi.devo4ka.top/kmi

Чтобы прочитать сообщение, перейдите по ссылке, которая будет выдана после отправки.

## Связь

https://devo4ka.top/