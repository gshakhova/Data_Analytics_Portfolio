## Описание проекта

Сервис аренды самокатов GoFast передал данные о некоторых пользователях из нескольких городов, а также об их поездках. Продакт-менеджеры сервиса хотят увеличить количество пользователей с подпиской. Для этого они будут проводить различные акции, но сначала нужно проверить несколько гипотез.

Чтобы совершать поездки по городу, пользователи сервиса GoFast пользуются мобильным приложением. Сервисом можно пользоваться:
* без подписки
    * абонентская плата отсутствует;
    * стоимость одной минуты поездки — 8 рублей;
    * стоимость старта (начала поездки) — 50 рублей.      
* с подпиской Ultra
    * абонентская плата — 199 рублей в месяц;
    * стоимость одной минуты поездки — 6 рублей;
    * стоимость старта — бесплатно.
    
*Цель исследования* - проанализировать данные и проверить гипотезы, которые могут помочь бизнесу вырасти.

*Задачи исследования:*

* описать и визуализировать общую информацию о пользователях и поездках;
* сравнить поведение пользователей с подпиской и без подписки;
* подсчитать помесячную выручку с каждого пользователя;
* проверить гипотезы.

*Ход исследования:*

В первую очередь изучим общую информацию о датафреймах, проверим данные на наличие пропусков и дубликатов, обработаем их, если такие значения присутствуют. Преобразуем столбец `date` в нужный тип datetime. Далее проведём исследовательский анализ данных: рассмотрим соотношение пользователей с подпиской и без, возраст пользователей, частоту встречаемости городов, расстояние и продолжительность поездок. Построим графики распределения для обозначенных параметров по двум категориям пользователей. Добавим столбец с помесячной выручкой, которую принёс каждый пользователь. В основной части исследования проверим следующие гипотезы:

* Продолжительность поездки (duration) пользователей с подпиской "Ультра" равна продолжительности поездки (duration) пользователей без подписки;
* Среднее расстояние одной поездки (distance) пользователей с подпиской "Ультра" = 3130 метров;
* Помесячная выручка (month_revenue) от пользователей с подпиской "Ультра" равна помесячной выручке (month_revenue) пользователей без подписки.

## Описание данных

1. Пользователи — users_go.csv:
   
* user_id	- уникальный идентификатор пользователя
* name - имя пользователя
* age	- возраст
* city - город
* subscription_type	- тип подписки (free, ultra)
   
2. Поездки — rides_go.csv:

* user_id	- уникальный идентификатор пользователя
* distance	- расстояние, которое пользователь проехал в текущей сессии (в метрах)
* duration	- продолжительность сессии (в минутах) — время с того момента, как пользователь нажал кнопку «Начать поездку» до момента, как он нажал кнопку «Завершить поездку»
* date	- дата совершения поездки

3. Подписки - subscriptions_go.csv:

* subscription_type	- тип подписки
* minute_price	- стоимость одной минуты поездки по данной подписке
* start_ride_price	- стоимость начала поездки
* subscription_fee	- стоимость ежемесячного платежа

## Библиотеки:

* Pandas
* Seaborn
* Matplotlib
* Numpy
* SciPy
* Math
