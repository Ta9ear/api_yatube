# api_yatube

## Описание:
API для проекта Yatube.

## Ресурсы API Yatube:

### 1)users:
Пользователи.
### 2) posts:
Посты.
### 3) groups:
Группы для постов.
### 4) follow:
Подписки на авторов.
### 5) comments:
Комментарии к постам.

## Установка

### 1) Клонировать репозиторий и перейти в директорию с проектом через терминал:
```
git clone git@github.com:Ta9ear/api_yatube.git
```

### 2) Cоздать и активировать виртуальное окружение:
```
python -m venv env
```
```
source venv/bin/activate
```

### 3) Установить зависимости из файла requirements.txt:
```
python -m pip install --upgrade pip
```
```
pip install -r requirements.txt
```

### 4)Выполнить миграции:
```
python manage.py migrate
```


### 5) Запустить проект:
```
python manage.py runserver
```

## Технологии
* Python
* Django
* DRF
* JWT
* Djoser

## Примеры запросов

GET запрос по адресу ниже выдаст список всех публикаций на сайте: 
```
http://127.0.0.1:8000/api/v1/posts/
```
POST запрос по этому же адресу позволит создать публикацию:
```
{
"text": "any text",
"group": "group id"
}
```
GET запрос по адресу ниже выдаст список всех комментариев к указанному id публикации:
```
http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/
```

### Автор проекта: Хусаенов Тагир
### Проект находится на стадии разработки

