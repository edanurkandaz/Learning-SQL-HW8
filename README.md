# Learning-SQL-HW8
www.patika.dev \
Aşağıdaki cümleleri SQL formatında yazalım. \
Veri tabanı olarak dvdrental'ı kullanalım. 


1-Test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım. \
CREATE TABLE employee ( \
	id INTEGER PRIMARY KEY, \
	name VARCHAR(50) NOT NULL, \
	birthday DATE, \
	email VARCHAR(100) \
); \
\
2-Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim. \
https://www.mockaroo.com/ \
![employee tablosuna 50 veri eklemek](https://user-images.githubusercontent.com/87134986/224374150-8b493774-cd98-4c70-8091-3a6590953de7.jpg)
\
\
3-Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım. \
UPDATE employee \
SET name = 'ayşe' \
WHERE id < 3; 

UPDATE employee \
SET name = 'eda' \
WHERE name LIKE 'u%'; 

UPDATE employee \
SET birthday = '1972-03-15' \
WHERE id = 5;

UPDATE employee \
SET name = 'ahmet' \
WHERE id > 48

UPDATE employee \
SET name = 'mehmet' \
WHERE email LIKE 't%';

4-Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım. \
DELETE FROM employee \
WHERE id < 11; 

DELETE FROM employee \
WHERE id = 8;

DELETE FROM employee \
WHERE name LIKE 'A%';

DELETE FROM employee \
WHERE email LIKE 'r%';

DELETE FROM employee \
WHERE id > 38;
