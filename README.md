
**Тестовое задание # 2 Работа с подписчиками одного издания.**

На сайте издания зарегистрировано 5 млн читателей, которые могут быть подписаны на любые из указанных изданий.
Читатель при регистрации вносили Имя и дату своего рождения.

Задание.
1. Необходимо создать структуру таблиц БД MySQL, учитывая все указанные параметры. Проставить индексы.
2. Составить запрос которым нужно будет получить   пользователей старше 30 лет только тех, кто подписан на журнал Мурзилка
3. Получить случайного 1-го пользователя из 5 млн, для отображения его в модуле “наш любимый читатель” на сайте.

## Решение задачи - быстрый старт

```
git clone git@github.com:ivanovsite/test.task.git
cd ./test.task
git checkout BookEdition
php -S 127.0.0.1:8000
http://127.0.0.1:8000/?edition=Мурзилка (не обязательный параметр edition - название журнала)
```
[ДЕМО](http://ivanov.site/demo/be/)

_Конечно если говорить о высоких нагрузках, больших обьемах данных и масштабировании, то здесь помимо кэширования, воркеров, балансировщиков ..., не обойтись без агрегирования данных, в данном случае это количество подписок по каждому читателю, количество читателей по каждому изданию._