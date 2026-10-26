1 Найди всех пользователей из Москвы или Берлина с помощью IN.

SELECT * FROM users
WHERE city IN ('Moscow', 'Berlin');

2 Найди пользователей возрастом от 22 до 31 года включительно с помощью BETWEEN.

SELECT * FROM users
WHERE age BETWEEN 22 AND 31;

3 Найди пользователей, чьи имена начинаются на J.

SELECT * FROM users
WHERE name LIKE 'J%';

4 Найди пользователей, чьи имена заканчиваются на букву a.

SELECT * FROM users
WHERE name LIKE '%a';

5 Найди пользователей, чьи имена начинаются на a, без учёта регистра, используя ILIKE.

SELECT * FROM users
WHERE name ILIKE 'a%';

6 Найди пользователей, возраст которых НЕ находится в диапазоне от 25 до 31 включительно.

SELECT * FROM users
WHERE age NOT BETWEEN 25 AND 31;