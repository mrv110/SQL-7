# SQL-Ödev7

1. Film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.
```
SELECT rating FROM film GROUP BY rating;
```
2. Film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.
```
SELECT replacement_cost,COUNT(*) FROM film GROUP BY replacement_cost HAVING COUNT(*) > 50;
```
3. Customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?
```
SELECT store_id, COUNT(*) FROM customer GROUP BY store_id;
```
4. City tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.
```
SELECT country_id, COUNT(*) FROM city GROUP BY country_id ORDER BY count(*) DESC;
-- country_id = 44, count = 60
```

<img width="165" alt="sql" src="https://github.com/mrv110/SQL-7/assets/74553882/574ba03b-3f4f-4d17-b13c-cd15792cc7a5">
