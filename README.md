### Домашнее задание к лекции «Проектирование БД. Связи. 3НФ»

## Задание 1
Обязательная часть

Будем развивать схему для музыкального сервиса.

Ранее было ограничение, что каждый исполнитель поет строго в одном жанре - пора убрать это ограничение. Исполнители могут петь в разных жанрах, как и одному жанру могут принадлежать несколько исполнителей.

Аналогичное ограничение было и с альбомами у исполнителей (альбом мог выпустить только один исполнитель). Теперь альбом могут выпустить несколько исполнителей вместе. Как и исполнитель может принимать участие во множестве альбомов.

С треками ничего не меняем, все так же трек принадлежит строго одному альбому.

Но появилась новая сущность - сборник. Сборник имеет название и год выпуска. В него входят различные треки из разных альбомов.

Обратите внимание: один и тот же трек может присутствовать в разных сборниках.

Задание состоит из двух частей:

  1. Спроектировать и нарисовать схему (как в первой домашней работе). Прислать изображение со схемой.
  2. Написать SQL-запросы, создающие спроектированную БД (как во второй домашней работе). Прислать ссылку на файл, содержащий SQL-запросы.

Примечание: можно прислать сначала схему, получить подтверждение, что схема верная и после этого браться за написание запросов.

### Домашнее задание к лекции «Select-запросы, выборки из одной таблицы»

## Задание 1

Заполните базу данных из предыдущего домашнего задания. В ней должно быть:

   1. не менее 8 исполнителей;
   2. не менее 5 жанров;
   3. не менее 8 альбомов;
   4. не менее 15 треков;
   5. не менее 8 сборников.

Внимание! Должны быть заполнены все поля каждой таблицы, в т.ч. таблицы связей (исполнителей с жанрами, исполнителей с альбомами, сборников с треками).

## Задание 2

Написать SELECT-запросы, которые выведут информацию согласно инструкциям ниже.
Внимание! Результаты запросов не должны быть пустыми (учтите при заполнении таблиц).

   1. название и год выхода альбомов, вышедших в 2018 году;
   2. название и продолжительность самого длительного трека;
   3. название треков, продолжительность которых не менее 3,5 минуты;
   4. названия сборников, вышедших в период с 2018 по 2020 год включительно;
   5. исполнители, чье имя состоит из 1 слова;
   6. название треков, которые содержат слово "мой"/"my".

Результатом работы будет 3 файла (с INSERT, SELECT запросами и CREATE запросами из предыдущего задания) в формате .sql (или .py/.ipynb, если вы будете писать запросы с использованием SQLAlchemy).
