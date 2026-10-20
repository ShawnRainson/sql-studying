Задание 1
SELECT name, age FROM users
ORDER BY age DESC;

Задание 2
SELECT * FROM users
ORDER BY city ASC, age ASC;

Задание 3
SELECT * FROM users
ORDER BY age ASC
LIMIT 2;

Задание 4
SELECT * FROM users
ORDER BY age ASC
OFFSET 2
LIMIT 2;

Задание 5 — проверка понимания
Выводит Ivan и John, сортирует по возрасту от старшего к младшему, пропускает одну строку и выводит две следующие

Задание 6 — боевое ⚔️
SELECT name, city, age FROM users
WHERE city = 'Kazan'
ORDER BY age DESC
LIMIT 1;	