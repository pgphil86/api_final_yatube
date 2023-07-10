# Hi there. This is project 'Api for Yatube' from Pavel.
```
https://github.com/pgphil86
```
![image](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=pgphil86&theme=dark)

![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)

### Languages:
### I. Русский язык.
### II. English language.

## I. Проект «API для Yatube»

### Описание проекта.
'API для Yatube' - это проект социальной сети. В котором есть возможность получения и редактирования постов, их комментариев, просмотр сообществ. Так же вы сможете подписаться на интересующего вас автора. В проекте используется JWT аутентификация. 

В проекте используются: Python 3.9, Django 3.2.16, Django Rest Framework (DRF) 3.12.4.

### Установка проекта.
Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/yandex-praktikum/api_final_yatube.git
```
```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:
```
python3 -m venv env
```
```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:
```
python3 -m pip install --upgrade pip
```
```
pip install -r requirements.txt
```

Выполнить миграции:
```
python3 manage.py migrate
```

Запустить проект:
```
python3 manage.py runserver
```

### Примеры возможностей проекта.
1. Создание, редактирование и удаление публикаций. Получение списка публикаций.
1. Просмотр сообществ и их списков.
1. Добавление комментария к публикации. Просмотр всех комментариев к публикации.
1. Подписка на публикации других пользователей проекта. И просмотр других подписчиков.

Первый пример, GET-запрос, при котором получаем список публикаций:
```
http://127.0.0.1:8000/api/v1/posts/
```
[
    {
        "id": 1,
        "text": "string",
        "author": "admin",
        "image": null,
        "group": null,
        "pub_date": "2023-07-10T20:11:54.322377Z"
    }
]

Второй пример, POST-запрос, позволяющий добавить новый комментарий к публикации:
```
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
```
{
    "id": 1,
    "author": "admin",
    "post": 1,
    "text": "some_string",
    "created": "2023-07-10T20:13:55.284220Z"
}

Третий пример, получение информации о сообществе по id:
```
http://127.0.0.1:8000/api/v1/groups/{id}/
```

Четвёртый пример, подписка пользователя на пользователя содержащегося в запросе:
```
http://127.0.0.1:8000/api/v1/follow/
```

## II. The 'API for Yatube' project

## Description of the project.
'API for Yatube' is a social network project. In which it is possible to receive and edit posts, their comments, and view communities. You can also subscribe to the author you are interested in. The project uses JWT authentication.

The project uses: Python 3.9, Django 3.2.16, Django Rest Framework (DRF) 3.12.4.

## Project installation.
Clone the repository and go to it on the command line:
```
git clone https://github.com/yandex-praktikum/api_final_yatube.git
```
```
cd api_final_yatube
```

Create and activate a virtual environment:
```
python3 -m venv env
```
```
source env/bin/activate
```

Install dependencies from a file requirements.txt:
```
python3 -m pip install --upgrade pip
```
```
pip install -r requirements.txt
```

Perform migrations:
```
python3 manage.py migrate
```

Launch a project:
```
python3 manage.py runserver
```

## Examples of project features.
1. Creating, editing and deleting publications. Getting a list of publications.
1. View communities and their lists.
1. Adding a comment to the publication. View all comments to the publication.
1. Subscribe to the publications of other users of the project. And view other subscribers.

First example, a GET request in which we get a list of publications:
```
http://127.0.0.1:8000/api/v1/posts/
```
[
    {
        "id": 1,
        "text": "string",
        "author": "admin",
        "image": null,
        "group": null,
        "pub_date": "2023-07-10T20:11:54.322377Z"
    }
]

Second example, a POST request that allows you to add a new comment to a post:
```
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
```
{
    "id": 1,
    "author": "admin",
    "post": 1,
    "text": "some_string",
    "created": "2023-07-10T20:13:55.284220Z"
}

Third example, getting information about a community by id:
```
http://127.0.0.1:8000/api/v1/groups/{id}/
```

Forth example, a user subscribing to a user contained in the request:
```
http://127.0.0.1:8000/api/v1/follow/
```
