## Дипломный проект по курсу «Django: создание функциональных веб-приложений»

Cайт интернет-магазина. Реализована клиентская часть сервиса и интерфейс администрирования.

## Описание клиентской части
Просмотр товара и добавление в корзину (рядом с каждым товаром должна быть кнопка добавления в корзину).
Кнопок добавления в корзину нет, если пользователь не авторизован
- Главная страница со статьями о подборке товаров (отсортированы по дате создания статьи) и перечислением этих товаров.
- Страница категории товара со списком товаров.
- Страница товара с подробным описанием, с возможность оставить отзыв (только для авторизованных пользователей).

## Меню:

- Ссылка на главную страницу.
- Ссылки на разделы (разделы могут иметь иерархию).
- Ссылка на корзину (только для авторизованных пользователей).
- Кнопка входа/выхода в зависимости от статуса авторизации.
- Корзина со списком выбранных товаров, привязанных к пользователю. Кнопка заказа создает заказ и очищает корзину.

Для входа - аутентификация по email'у.

## Интерфейс администратора

- Редактирование разделов.
- Редактирование товаров.
- Редактирование статей на главной странице и привязывание к ним товаров, которые должны отображаться после нее.
- Просмотр списка заказов пользователей, отсортированных по дате создания, с указанием пользователя и количества товаров.
- Страница детализации заказа с просмотром списка заказанных товаров.

## Требования к организации системы

- Система реализована на Django версии 2.
- Интерфейс администратора создан стандартными средствами Django admin.
- В качестве СУБД использовать sqlite.

## Для запуска проекта необходимо выполнить команды:

Провести миграцию:

```bash
python manage.py migrate
```
Для загрузки начальных данных модели Book необходимо выполнить команду:

```bash
python manage.py loaddata fixtures.json
```
Запустить отладочный веб-сервер проекта:

```bash
python manage.py runserver
```

Суперпользователь с именем admin и паролем admin
