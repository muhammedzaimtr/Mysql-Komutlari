# Mysql-Komutlari
Mysql komutları nasıl kullanılır falan filan Sürekli Olarak Güncellenecektir... 

**SQL Nedir? Ne Değildir?**
---------------------------

SQL ‘in diğer bir adı ise yapılandırılmış sorgulama dilidir. SQL kısaca anlatmak gerekirse verileri yönetmek ve tasarlamak için kullanılan veritabanı yönetim sistemidir. Şunu bilmeniz gerekiyor ki SQL bir programlama dili değildir…

<br><br>
----------


**Veritabanı Oluşturma ve Veritabanı seçme**

**Veritabanı oluşturma komutu:**

> Create Database veritabaniismi ;

<br><br>
----------


**Veritabanı Seçme Komutu:**

> Use veritabanıismi;

<br><br>
----------


**Tablo Oluşturma**

**Tablo oluşturma komutu:**

> Create table tabloadi (
> 
> alanadi1 veritipi,
> 
> alanadi2 veritipi
> 
> );

<br><br>
----------


**Tabloya Veri Girişi Yapmak**

**Veri girişi komutu:**

> insert into tabloadi (alandi1,alanadi2,alanadi3) values
> (“veri1“,”veri2“,”veri3“);


----------


**Tablo Üzerinde Değişiklik Yapmak**

**Tabloya yeni alan ekleme komutu:**

> alter table tabloadi add alanadi veritipi ;


----------


**Tablodaki alan üzerinde değişiklik yapma komutu:**

> alter table tabloadi alter column alanadi veritipi;


----------


**Var olan tablodan alan silme komutu:**

> alter table tabloadi drop alanadi;


----------


**Tabloya Kısıtlama Ekleme**

> **“not null”** veri tanımsız yani boş olamaz demektir.
> **“unsigned”** veri değeri bir tam sayı olmak zorundadır anlamına gelir.
> **“auto_increment”** kodlama dillerinde sütuna boş bir değer tanımlandığında otomatik olarak değeri oluşturur ve tanımlanır.
> **“primary key”** Birincil anahtar anlamına gelir.Tablo’nun birincil sütunudur ve her zaman farklıdır.


----------


**MySQL komutlarının kullanımı ise aşağıdaki şekildedir.**

> CREATE TABLE uyelik 
> ( 
> id INT AUTO_INCREMENT PRIMARY KEY,
>  ad VARCHAR(50) not null,
>   yas INT, 
> );


----------


**Tablo Silme**

> drop table tabloadi;


----------


**Tablodan alan silme**

**alter table tabloadi drop alanadi;**


----------


**Tablodan Veri Listeleme**

> select * from  tabloadi; *#tablodaki tüm alanları listeler*
> 
> select alan1,alan2 from tabloadi; *#tablodaki seçilen alanlari listeler*


----------


**Tekrarlı Kayıtları Kaldırma**

> Select distinct alanadi from tabloadi;


----------


**Alanlara Takma Ad Ekleme**

> Select alanadi astakmaadfromtabloadi;


----------


**Tablodan veri silme**

> Delete fromtabloadi;


----------


**Var olan kayıtları güncelleme**


> update tabloadi set güncellenecekveri where sart;


----------


**Not Operatörü kullanımı**

> Select *from tabloadi where not (dahil edilmek istenmeyen değerlerin
> geleceği yer);


----------


**İn Operatörü kullanımı**

> Select * from tabloadi where in(veri1,veri2);


----------


**Between Operatörü kullanımı**

> Select  * from tabloadi where alanadi between değer1 and değer2;


----------


**Order by Operatörü kullanımı**

> Select  * from tabloadi where order by alanadi asc/desc;
> 
> desc = büyükten küçüğe sıralama
> 
> asc = küçükten büyüğe sıralama


----------


**Concat Operatörü kullanımı**

> Select  concat(ad , soyad ) as advesoyad from tabloadi ;


----------


**Lenght Operatörü kullanımı**

> Select  lenght(ad  ) as adınuzunluğu from tabloadi ;


----------


**Lower ve Upper Operatörü kullanımı**

> Select  lower / upper (ad ) as buyukveyakuçukhali from tabloadi ;


----------


**Ltrim ve Rtrim Operatörü kullanımı**

> Select  ltrim / rtrim (ad ) as boşluksilme from tabloadi ;


----------


**Lower ve Upper Operatörü kullanımı**

> Select  lower(ad ) as takmaad from tabloadi ;


----------


**Substring Operatörü kullanımı**

> select substring(ad,1,5) as Say from personel;


----------


**AVG Operatörü kullanımı**

> select avg(maas) as ortalamamaas from personel;


----------


**Sum Operatörü kullanımı**

> select sum(maas) as toplammaas from personel;


----------


**Max ve Min Operatörü kullanımı**

> select max(maas) as enyüksekmaas from personel;
> 
> select min(maas) as endusukmaas from personel;


----------


**Concat Operatörü kullanımı**

> select ad,soyad,concat(ad,soyad,”@gmail.com“) from personel;

 


----------

Güncelleniyor...
================


----------
