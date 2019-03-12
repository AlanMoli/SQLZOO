## SELECT basics
### 1. Introducing the world table of countries
```SQL
SELECT population 
FROM world
WHERE name = 'Germany';
```

### 2. Scandinavia
```SQL
SELECT name, population 
FROM world
WHERE name IN ('Sweden', 'Norway', 'Denmark');
```

### 3. Just the right size
```SQL
SELECT name, area 
FROM world
WHERE area BETWEEN 200000 AND 250000；
```