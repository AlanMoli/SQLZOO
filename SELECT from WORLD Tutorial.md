## SELECT from WORLD Tutorial
### 1. Introduction
```SQL
SELECT name, continent, population FROM world
```

### 2. Large Countries
```SQL
SELECT name FROM world
WHERE population >= 200000000;
```

### 3. Per capita GDP
```SQL
SELECT name, gdp/population
FROM world
WHERE population >= 200000000;
```

### 4. South America In millions
```SQL
SELECT name, population/1000000
FROM world
WHERE continent = 'South America';
```

### 5. France, Germany, Italy
```SQL
SELECT name, population
FROM world
WHERE name in ('France', 'Germany', 'Italy');
```

### 6. United
```SQL
SELECT name
FROM world
WHERE name LIKE '%United%';
```

### 7. Two ways to be big
```SQL
SELECT name, population, area
FROM world 
WHERE area/1000000 > 3 
 OR population/1000000 > 250;
```