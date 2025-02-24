# API для социальной сети Yatube

## Описание
Проект создан в рамках учебного курса Яндекс.Практикум.

API сервис для проекта социальной сети Yatube.


#### Доступный функционал
- Python 3.9
- Works on Linux, Windows, macOS
- Django 3.2
- Django Rest Framework
- Pytest
- Simple-JWT
- SQLite3


Запуск проекта в dev-режиме()
----------

1. Клонировать репозиторий и перейти в него в командной строке:
```bash
git clone git@github.com:Kostrulnik/api_yatube.git

cd api_yatube
```
2. Cоздать и активировать виртуальное окружение:
```bash
python -m venv venv

source venv/bin/activate
```
3. Установить зависимости из файла ```requirements.txt```:
```bash
python -m pip install --upgrade pip

pip install -r requirements.txt
```
4. Выполнить миграции:
```bash
python manage.py migrate
```
5. Запустить проект:
```bash
python manage.py runserver
```
----------
Примеры некоторых запросов API
----------
Получить список всех постов:  
``` GET /api/v1/posts/ ```  
Добавление нового поста:  
``` POST /api/v1/posts/ ```   
Получить список всех групп:  
``` GET /api/v1/groups/ ```  
Получить информацию о группе по id
```GET /api/v1/groups/{group_id}/```
Добавление нового комментария:  
``` POST /api/v1/posts/{post_id}/comments/ ```  
Удаление комментария по id:  
``` DELETE /api/v1/posts/{post_id}/comments/{id}/ ```
Получение списока подписок:  
``` GET /api/v1/follow/ ```  
Подписка пользователя на пользователя переданного в запросе:  
``` POST /api/v1/follow/ ```  

Документация к проекту
---------
Документация к API доступна по адресу [http://127.0.0.1:8000/redoc/](http://127.0.0.1:8000/redoc/) после запуска сервера с проектом

Автор
----------
Головко Константин - [https://github.com/Kostrulnik](https://github.com/Kostrulnik)