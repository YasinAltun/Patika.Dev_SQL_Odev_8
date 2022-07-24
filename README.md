# Patika.Dev_SQL_Odev_8
POSTRGRESQL - Tablo Oluşturmak - Silmek - Verileri Güncellemek - Silmek

Merhabalar,

1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.

2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.

4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.

Kolay Gelsin.


# ÇÖZÜMLER

## 1.test veritabanınızda employee isimli sütun bilgileri id(INTEGER), name VARCHAR(50), birthday DATE, email VARCHAR(100) olan bir tablo oluşturalım.
'''
CREATE TABLE employee(
	id serial ,
	name varchar(50) ,
	birthday date,
	email varchar(100)
);

'''
## 2.Oluşturduğumuz employee tablosuna 'Mockaroo' servisini kullanarak 50 adet veri ekleyelim.

insert into employee (name, birthday, email) values ('Rod', '1954-06-21', 'rpenniall0@bloomberg.com');
insert into employee (name, birthday, email) values ('Marge', '1989-08-21', 'mfreyne1@usda.gov');
insert into employee (name, birthday, email) values ('Dana', '2002-01-23', 'dlembke2@w3.org');
insert into employee (name, birthday, email) values ('Grenville', '2016-12-24', 'gulyat3@mit.edu');
insert into employee (name, birthday, email) values ('Meredithe', '2002-08-03', 'mrickford4@tmall.com');
insert into employee (name, birthday, email) values ('Prissie', '2019-08-06', 'pdeddum5@youtube.com');
insert into employee (name, birthday, email) values ('Rheba', '2009-06-29', 'rdelaspee6@washington.edu');
insert into employee (name, birthday, email) values ('Minna', '1970-02-22', 'mwince7@wikia.com');
insert into employee (name, birthday, email) values ('Ellen', '1961-03-14', 'edeware8@howstuffworks.com');
insert into employee (name, birthday, email) values ('Elwin', '1958-12-26', 'eglazyer9@engadget.com');
insert into employee (name, birthday, email) values ('Lacee', '2006-02-27', 'lbutlerbowdona@360.cn');
insert into employee (name, birthday, email) values ('Dirk', '1995-09-01', 'dnagleb@ifeng.com');
insert into employee (name, birthday, email) values ('Em', '2007-08-18', 'ecatterallc@cnn.com');
insert into employee (name, birthday, email) values ('Florette', '1993-12-29', 'fscranneyd@sitemeter.com');
insert into employee (name, birthday, email) values ('Deloris', '1952-07-23', 'dbesemere@facebook.com');
insert into employee (name, birthday, email) values ('Berti', '1964-06-15', 'bbanglef@sitemeter.com');
insert into employee (name, birthday, email) values ('Britney', '1998-04-12', 'bnecoldsg@diigo.com');
insert into employee (name, birthday, email) values ('Burton', '2020-04-28', 'bwallaceh@canalblog.com');
insert into employee (name, birthday, email) values ('Staffard', '1999-01-02', 'sarmatagei@mtv.com');
insert into employee (name, birthday, email) values ('Christian', '1951-11-14', 'cprescottj@wufoo.com');
insert into employee (name, birthday, email) values ('Roderigo', '1996-10-21', 'rbingallk@opera.com');
insert into employee (name, birthday, email) values ('Harriet', '1995-10-25', 'hcecchil@squarespace.com');
insert into employee (name, birthday, email) values ('Windy', '2006-09-27', 'wclementetm@columbia.edu');
insert into employee (name, birthday, email) values ('Tobe', '1995-06-28', 'tgyfordn@tripadvisor.com');
insert into employee (name, birthday, email) values ('Tiphany', '1972-11-15', 'tdibdino@answers.com');
insert into employee (name, birthday, email) values ('Garfield', '2012-01-04', 'grumseyp@parallels.com');
insert into employee (name, birthday, email) values ('Hedy', '2006-07-17', 'hiacopoq@github.io');
insert into employee (name, birthday, email) values ('Francesco', '1974-06-21', 'fabisettir@trellian.com');
insert into employee (name, birthday, email) values ('Aveline', '1958-06-19', 'arackhams@alexa.com');
insert into employee (name, birthday, email) values ('Emogene', '1958-10-11', 'estoakt@acquirethisname.com');
insert into employee (name, birthday, email) values ('Jack', '1951-03-25', 'jgluyusu@facebook.com');
insert into employee (name, birthday, email) values ('Filberto', '1970-04-24', 'fcoanv@taobao.com');
insert into employee (name, birthday, email) values ('Royal', '1973-11-23', 'rshielw@weibo.com');
insert into employee (name, birthday, email) values ('Otto', '2008-06-09', 'obroganx@timesonline.co.uk');
insert into employee (name, birthday, email) values ('Rae', '2000-12-01', 'rstickingsy@ehow.com');
insert into employee (name, birthday, email) values ('Theressa', '2019-01-18', 'tolochanz@deliciousdays.com');
insert into employee (name, birthday, email) values ('Franky', '2003-07-29', 'fruddock10@noaa.gov');
insert into employee (name, birthday, email) values ('Warren', '2008-06-11', 'wfronek11@foxnews.com');
insert into employee (name, birthday, email) values ('Delmore', '1959-05-23', 'dbyres12@exblog.jp');
insert into employee (name, birthday, email) values ('Hussein', '1965-12-10', 'hricca13@sohu.com');
insert into employee (name, birthday, email) values ('Whittaker', '1979-12-14', 'wleyland14@cafepress.com');
insert into employee (name, birthday, email) values ('Nanni', '1984-11-12', 'ndumbar15@wunderground.com');
insert into employee (name, birthday, email) values ('Mathew', '2002-03-20', 'mflatt16@state.gov');
insert into employee (name, birthday, email) values ('Nicolis', '1980-06-23', 'nmccullum17@fotki.com');
insert into employee (name, birthday, email) values ('Bernarr', '2016-02-03', 'bpearton18@qq.com');
insert into employee (name, birthday, email) values ('Atlante', '1952-05-22', 'adeshon19@friendfeed.com');
insert into employee (name, birthday, email) values ('Christalle', '2008-09-04', 'crattry1a@studiopress.com');
insert into employee (name, birthday, email) values ('Joice', '1971-07-15', 'jkeepin1b@freewebs.com');
insert into employee (name, birthday, email) values ('Cati', '1961-09-24', 'cfrake1c@wisc.edu');
insert into employee (name, birthday, email) values ('Clari', '1974-03-11', 'cwittleton1d@biblegateway.com');

## 3.Sütunların her birine göre diğer sütunları güncelleyecek 5 adet UPDATE işlemi yapalım.


## 4.Sütunların her birine göre ilgili satırı silecek 5 adet DELETE işlemi yapalım.



İYİ ÇALIŞMALAR
