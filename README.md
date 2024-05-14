# SQLodev7
## sql sorguları patika odev 7 ##
**Aşağıdaki sorgu senaryolarını dvdrental örnek veri tabanı üzerinden gerçekleştiriniz.**<br/>
1.film tablosunda bulunan filmleri rating değerlerine göre gruplayınız.<br/><br/>
SELECT rating,title from film<br/>
group by rating,title;<br/><br/><br/>
2.film tablosunda bulunan filmleri replacement_cost sütununa göre grupladığımızda film sayısı 50 den fazla olan replacement_cost değerini ve karşılık gelen film sayısını sıralayınız.<br/><br/>
SELECT replacement_cost,count(*) from film<br/>
group by replacement_cost<br/>
having  count(*)>=50<br/>
order by replacement_cost,count(*);<br/><br/><br/>
3.customer tablosunda bulunan store_id değerlerine karşılık gelen müşteri sayılarını nelerdir?<br/><br/>
SELECT store_id,count(*) from customer<br/>
group by store_id;<br/><br/>
4.city tablosunda bulunan şehir verilerini country_id sütununa göre gruplandırdıktan sonra en fazla şehir sayısı barındıran country_id bilgisini ve şehir sayısını paylaşınız.<br/><br/>
SELECT country_id,count(*) from city<br/>
group by country_id<br/>
ORDER BY count(*) DESC<br/>
LIMIT 1;<br/><br/>

