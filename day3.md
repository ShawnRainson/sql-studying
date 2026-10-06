Задание 1
Получить пользователей старше 30 лет.

SELECT * FROM users
WHERE age > 30;

Задание 2
Получить пользователей, которые не из Казани.

SELECT * FROM users
WHERE city = 'Kazan';

Задание 3
Получить пользователей:
- младше 30 лет;
- из Москвы.

SELECT * FROM users
WHERE city = 'Moscow'
AND age < 30;

Задание 4
Получить пользователей:
- из Москвы или Казани;
- возрастом 30 лет или старше.
Используй скобки.

SELECT * FROM users
WHERE (city = 'Moscow' OR city = 'Kazan')
AND age >= 30;

Задание 5 — проверка мышления 🧠
Какой результат даст этот запрос?
SELECT name
FROM users
WHERE age >= 25
  AND city = 'Moscow'
   OR city = 'Berlin';

Не запускай его.
Напиши, какие имена, по-твоему, вернёт PostgreSQL и почему. - Выдаст пользователей от 25 включительно и выше из Москвы.

⚔️ Задание 6 — боевое
Напиши запрос:
Получить name, age и city пользователей, которые не из Москвы, старше 25 лет, но не старше 35 лет. Отсортировать по возрасту от старшего к младшему.

SELECT name, age, city FROM users
WHERE city <> 'Moscow'
AND age > 25 AND age < 35
ORDER BY age DESC;

