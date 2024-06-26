## Описание проекта

Интернет-магазин «Стримчик» продаёт по всему миру компьютерные игры. Из открытых источников доступны исторические данные о продажах игр, оценки пользователей и экспертов, жанры и платформы (например, Xbox или PlayStation).

*Цель исследования* - выявить определяющие успешность игры закономерности.

*Задачи исследования:*

* сравнить продажи по платформам в динамике и выявить актуальный период для целей прогнозирования продаж;
* составить портрет пользователя каждого региона;
* проверить гипотезы про пользовательские рейтинги.

*Ход исследования:*

В первую очередь откроем файл и подготовим данные для анализа. Заменим некорректные названия столбцов, преобразуем данные в нужные типы, обработаем пропуски и проверим наличие дубликатов и аномалий. В разделе исследовательский анализ данных посмотрим, как менялись продажи по платформам и определим их "жизненный срок". На основе полученных результатов выявим актуальный период для целей прогнозирования продаж. Далее рассмотрим жанры с высокой и низкой прибылью, а также оценим корреляцию между отзывами и продажами. 

Определим для пользователей каждого региона:

* самые популярные платформы (топ-5);
* самые популярные жанры (топ-5);
* как влияет рейтинг ESRB на продажи.

В основной части исследования проверим следующие гипотезы: 

* Средние пользовательские рейтинги платформ Xbox One и PC одинаковые;
* Средние пользовательские рейтинги жанров Action (англ. «действие», экшен-игры) и Sports (англ. «спортивные соревнования») разные.

В конце напишем общий вывод по результатам анализа. 

Результаты исследования позволят понять, на какой потенциально популярный продукт сделать ставку и спланировать рекламные кампании. В нашем распоряжении данные до 2016 года. Представим, что сейчас декабрь 2016 г., и мы планируем кампанию на 2017-й. Нужно отработать принцип работы с данными. Неважно, прогнозируем ли мы продажи на 2017 год по данным 2016-го или же 2027-й — по данным 2026 года.

В наборе данных попадается аббревиатура ESRB (Entertainment Software Rating Board) — это ассоциация, определяющая возрастной рейтинг компьютерных игр. ESRB оценивает игровой контент и присваивает ему подходящую возрастную категорию, например, «Для взрослых», «Для детей младшего возраста» или «Для подростков».

## Описание данных

* Name — название игры
* Platform — платформа
* Year_of_Release — год выпуска
* Genre — жанр игры
* NA_sales — продажи в Северной Америке (миллионы проданных копий)
* EU_sales — продажи в Европе (миллионы проданных копий)
* JP_sales — продажи в Японии (миллионы проданных копий)
* Other_sales — продажи в других странах (миллионы проданных копий)
* Critic_Score — оценка критиков (максимум 100)
* User_Score — оценка пользователей (максимум 10)
* Rating — рейтинг от организации ESRB (англ. Entertainment Software Rating Board). Эта ассоциация определяет рейтинг компьютерных игр и присваивает им подходящую возрастную категорию.

Данные за 2016 год могут быть неполными.

## Библиотеки:

* Pandas
* Seaborn
* Matplotlib
* Numpy
* SciPy
