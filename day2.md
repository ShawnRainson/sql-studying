Задание 1

Получить только имена:

SELECT name
FROM users;

Задание 2

Получить name и city.
SELECT name, city
FROM users;

Задание 3

Получить name и возраст, но назвать возраст user_age.
SELECT name, age AS user_age
FROM users;

Задание 4

Получить имя и возраст плюс один год, назвать результат age_next_year.
SELECT name, age AS age_next_year = age + 1
FROM users;

Задание 5 — боевое ⚔️

Напиши запрос, который получает:

имя;
город;
только пользователей из Kazan;
отсортированных по возрасту от старшего к младшему

SELECT name, city FROM users
WHERE city = 'Kazan'
ORDER BY age DESC;

🧠 Мини-тест Дня 2

Без запуска PostgreSQL. Ответь своими словами или SQL.

1.

Что делает:

SELECT *
FROM users;
Выводит все столбцы из таблицы users

2.

В чём разница между:

SELECT age - обычный вывод age
FROM users;

и

SELECT age AS user_age - вывод age под псевдонимом
FROM users;

3.

Что вернёт:

SELECT name, age + 5 AS future_age - вывод возрастов увеличенный на 5
FROM users;

Изменится ли значение age в самой таблице? - нет

4.

Исправь ошибку:

SELECT name, age
FROM users;

Нужно получить два столбца: name и age.

⚔️ Финальный раунд

Напиши запрос:

Получить имя и возраст пользователей из Москвы, показать возраст как user_age, отсортировать от самого старшего к самому младшему и показать максимум 2 строки.

Вот тут уже собери всё сегодняшнее и вчерашнее в один запрос. 👊

SELECT name, age AS user_age FROM users
WHERE city = 'Moscow'
ORDER BY age DESC
LIMIT 2;