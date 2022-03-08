# sqlHomeWork4 Patika.dev SQL Modülü Ödevleri  Aşağıdaki sorgu senaryoları dvdrental örnek veri tabanı üzerinden gerçekleştirilmiştir.
`Soru`
film tablosunda bulunan replacement_cost sütununda bulunan birbirinden farklı değerleri sıralayınız.
```sql
SELECT DISTINCT replacement_cost 
FROM film;
```
`Soru`
film tablosunda bulunan replacement_cost sütununda birbirinden farklı kaç tane veri vardır?
```sql
SELECT  COUNT(DISTINCT replacement_cost) 
FROM film;
```
`Soru`
film tablosunda bulunan film isimlerinde (title) kaç tanesini T karakteri ile başlar ve aynı zamanda rating 'G' ye eşittir?
```sql
SELECT COUNT(title)
FROM film 
WHERE title LIKE 'T%' AND rating='G';
```
`Soru`
country tablosunda bulunan ülke isimlerinden (country) kaç tanesi 5 karakterden oluşmaktadır?
```sql
SELECT COUNT(country) 
FROM country
WHERE country LIKE '_____%';
```
`Soru`
city tablosundaki şehir isimlerinin kaç tanesi 'R' veya r karakteri ile biter?
```sql
SELECT COUNT (title) 
FROM city
WHERE title LIKE '%R' OR '%r';
```
