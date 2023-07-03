<img src="https://global-uploads.webflow.com/6097e0eca1e875de53031ff6/6241a5ec363584013b7b1857_Patika%20logo%20(2).png" alt="patika image" height="200px" width="200px">

# PATIKA HOMEWORKS

## Homework 1

<br><br>

1-) Film tablosunda bulunan title ve description sütunlarındaki verileri sıralayınız.


```
SELECT title, description FROM film;

```
<br>

2-) Film tablosunda bulunan tüm sütunlardaki verileri film uzunluğu (length) 60 dan büyük VE 75 ten küçük olma koşullarıyla sıralayınız.


```
SELECT * FROM film
WHERE length > 60 AND length < 75;

```
<br>

3-) Film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99 VE replacement_cost 12.99 VEYA 28.99 olma koşullarıyla sıralayınız.


```
SELECT * FROM film
WHERE rental_rate = 0.99 AND (replacement_cost=12.99 OR  replacement_cost=28.99);

```
<br>

4-) customer tablosunda bulunan first_name sütunundaki değeri 'Mary' olan müşterinin last_name sütunundaki değeri nedir?

```
SELECT last_name FROM customer
WHERE first_name='Mary';

```
<br>

5-) film tablosundaki uzunluğu(length) 50 ten büyük OLMAYIP aynı zamanda rental_rate değeri 2.99 veya 4.99 OLMAYAN verileri sıralayınız.

```
SELECT * FROM film
WHERE (NOT length>50) AND NOT( rental_rate = 2.99 OR rental_rate = 4.99)

```
<br><br>

## Homework 2

1-) film tablosunda bulunan tüm sütunlardaki verileri replacement cost değeri 12.99 dan büyük eşit ve 16.99 küçük olma koşuluyla sıralayınız ( BETWEEN - AND yapısını kullanınız.)
```
SELECT * FROM film
WHERE replacement_cost BETWEEN 12.99 AND 16.99

```
<br>

2-) actor tablosunda bulunan first_name ve last_name sütunlardaki verileri first_name 'Penelope' veya 'Nick' veya 'Ed' değerleri olması koşuluyla sıralayınız. ( IN operatörünü kullanınız.)
```
SELECT first_name , last_name FROM actor
WHERE first_name IN('Penelope','Nick','Ed')

```
<br>

3-) film tablosunda bulunan tüm sütunlardaki verileri rental_rate 0.99, 2.99, 4.99 VE replacement_cost 12.99, 15.99, 28.99 olma koşullarıyla sıralayınız. ( IN operatörünü kullanınız.)

```
SELECT *  FROM film
WHERE rental_rate IN(0.99, 2.99, 4.99) AND replacement_cost IN(12.99, 15.99, 28.99)

```
