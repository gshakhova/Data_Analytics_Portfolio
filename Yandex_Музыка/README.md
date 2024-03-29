## Описание проекта

Сравнение Москвы и Петербурга окружено мифами. Например:
 * Москва — мегаполис, подчинённый жёсткому ритму рабочей недели;
 * Петербург — культурная столица, со своими вкусами.
 
*Цель исследования* - сравнить поведение пользователей двух столиц на данных Яндекс Музыки.

*Задача исследования* - проверить три гипотезы:

* Активность пользователей зависит от дня недели. Причём в Москве и Петербурге это проявляется по-разному.
* В понедельник утром в Москве преобладают одни жанры, а в Петербурге — другие. Так же и вечером пятницы преобладают разные жанры — в зависимости от города. 
* Москва и Петербург предпочитают разные жанры музыки. В Москве чаще слушают поп-музыку, в Петербурге — русский рэп.

*Ход исследования:*

Перед проверкой гипотез проведём проверку данных на наличие пропусков и дубликатов. Оценим их влияние на исследование. Далее проверим наши гипотезы.  

Таким образом, исследование пройдёт в три этапа:
 1. Обзор данных.
 2. Предобработка данных.
 3. Проверка гипотез.

## Данные

Описание колонок:

* userID — идентификатор пользователя;
* Track — название трека;
* artist — имя исполнителя;
* genre — название жанра;
* City — город пользователя;
* time — время начала прослушивания;
* Day — день недели.

## Библиотеки:

* Pandas
