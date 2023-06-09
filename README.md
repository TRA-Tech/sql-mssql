# SQL
SQL (Structured Query Language), ilişkisel veritabanı yönetim sistemlerinde kullanılan bir programlama dilidir. SQL, veritabanlarında veri eklemek, güncellemek, silmek ve sorgulamak için kullanılır.

SQL, 1970'lerde IBM tarafından geliştirilmiş ve daha sonra ANSI (American National Standards Institute) ve ISO (International Organization for Standardization) tarafından standartlaştırılmıştır. SQL, ilişkisel veritabanı yönetim sistemleri (RDBMS) için özellikle tasarlanmıştır ve birçok RDBMS, özellikle Oracle, MySQL, MSSQL, PostgreSQL ve SQLite tarafından desteklenir.

SQL, basit ve kolay anlaşılır bir dil olması nedeniyle çok yaygın olarak kullanılır. SQL sorguları, veritabanlarına erişmek için kullanılan birçok uygulamada kullanılabilir. SQL, veritabanlarında veri işleme işlemlerini otomatikleştirmeye ve hızlandırmaya yardımcı olan birçok özellik ve fonksiyona sahiptir. SQL sorguları, veritabanı işlemlerini gerçekleştirmek için tasarlanmıştır ve sorguların sonuçları, veritabanında depolanan verilerin bir görüntüsünü oluşturur.
<br>
<br>
Veritabanı yaklaşımı ile birlikte bir veri sorgulama diline veya aracına ihtiyaç duyulmuştur. İlk başta matematiksel bir sözdizimine sahip olan SQUARE adlı bir dil geliştirilmiştir. Geniş kullanıcı kitleleri tarafında kolay kullanılabilmesi için matematiksel söz dizimli SQUARE dilinden vazgeçilerek, İngilizceye benzer sözdizimine sahip bir dil oluşturulmuş ve SEQUEL olarak adlandırılmıştır. Daha sonra da bu SEQUEL dili, İngilizce söylenişine paralel olarak SQL olarak adlandırılmıştır.

SQL dili ilişkisel alanda büyük ilgi görmüş ve İlişkisel Veri Tabanı Yönetim Sistemlerinin (İVTYS) tümünde yer alan standart dil görünümü kazanmıştır. Bu nedenle Veri Tabanı konusunda çalışan tüm bilişim teknik personeli tarafından bilinmesi gereken bir dil konumundadır.
<br>

## SQL dilini kullanan veritabanları
- Sybase 
- MySQL
- PostgreSQL
- Microsoft SQL Server
- Oracle
- IBM DB2
- IBM Informix
- Progress
- Firebird
- Microsoft Access

<br>


## SQL sorguları 4 ana gruba ayrılır:
- DDL (Data Defination Language)
- DML (Data Manipulation Language)
- DCL (Data Control Language)
- TCL (Transaction Control Language)
![Untitled](https://github.com/TRA-Tech/sql-sqlserver/assets/100773960/7e0d9581-0c43-4d16-89a8-d7febf1e9645)

### DDL (Data Defination Language)


DDL yani **Veri Tanımlama Dili** verinin ne olduğu ile ilgilenmez. Verinin nerede, nasıl tutulacağı ile ilgilenir. Veritabanımıza kullanıcı ve tablo eklemek, güncellemek veya silmek gibi işlemler için DDL kullanırız.

En temel DDL komutları şu şekildedir:
- **CREATE** — Veritabanında tablo oluşturmamızı sağlar.
- **ALTER** — Veritabanınında ilgili tablo üzerinde değişiklik yapmamızı sağlar.
- **DROP** — Veritabanında ilgili tabloyu siler.
- **TRUNCATE** — Veritabanında ilgili tablodaki tüm kayıtları siler.
- **RENAME** — Veritabanında ilgili tabloyu yeniden adlandırır.

### DML (Data Manipulation Language)

DML yani **Veri İşleme Dili** veritabanındaki tablolar içerisindeki verileri yönetmek (ekleme, güncelleme, silme, seçme) için kullanılır.

En temel DML komutları şu şekildedir
- **SELECT** — Veritabanında ilgili tablodan veri çekmek/seçmek için kullanılır.
- **INSERT** — Veritabanında ilgili tabloya veri ya da verileri eklemek için kullanılır.
- **UPDATE** — Veritabanında ilgili tablodaki veri ya da verileri güncellemek için kullanılır.
- **DELETE** — Veritabanında ilgili tablodaki veri ya da verileri silmek için kullanılır.


### DCL (Data Control Language)

DCL yani **Veri Kontrol Dili** verilerden ziyade veritabanındaki kullanıcılar ile ilgilenir diyebiliriz. Hangi tabloya kimler erişebilir vb.

En temel DCL komutları şu şekildedir
- **GRANT** — Kullanıcıların veritabanındaki tablolar üzerinde işlem yapıp yapamayacağını belirlememizi sağlar. Kullanıcıya izin vermeye yarar.
- **DENY** — Kullanıcıların veritabanındaki tablolardaki verileri kullanmasını kısıtlamamızı sağlar. Kullanıcının yetkilerini geri almamıza yarar.
- **REVOKE** — Kullanıcıların veritabanında daha önce verilmiş izinlerini veya uygulanmış kısıtlamalarını kaldırmamızı sağlar.

### TCL (Transaction Control Language)


TCL yani **İşlem Kontrol Dili** de verilerden ziyade yapılan işlemler ile ilgilenmektedir. Örnek olarak veritabanına bir veri ekledik fakat TCL yardımı ile yaptığımız bu işlemi veritabanına bildirmedik/onaylamadık. Veritabanı yönetim programını kapatıp açtığımız zaman eklediğimiz verinin kayıt olmadığını göreceğiz. Bu gibi problemlerle karşılaşmamak için TCL kullanırız.

Muhtemelen çoğumuzun Entity Framework’den bildiği DbContext sınıfının ‘SaveChanges()’ metodu TCL’e bir örnektir (COMMIT).

En temel TCL komutları şu şekildedir.
- **COMMIT** — Veritabanında yaptığımız değişiklikleri onaylamamızı sağlar. Bu sayede yapılan değişiklikler (DML) veritabanına kayıt edilecektir.
- **SAVEPOINT** — Veritabanında daha sonra geri dönülecek bir dönüş noktası belirler. Bir nevi snapshot gibi düşünebiliriz.
- **ROLLBACK** — Veritabanımıza yanlışlıkla veri eklediğimizi ve COMMIT ile değişikliği veritabanına yazdığımızı düşünelim. Böyle bir senaryoda ROLLBACK kullanmamız gerekecektir. Şu anki COMMIT’ten bir önceki COMMIT’e geri dönmemizi sağlar bu sayede yanlışlıkla onayladığımız işlem aslında hiç olmamış gibi düşünebiliriz. Git versiyon kontrol sistemindeki reset komutuna benzetebiliriz (bkz:git reset).

Örnek olması adına aşağıda basit bir tablo oluşturmak için kullanılan kod parçasını görebiliriz.
``` sql
CREATE TABLE Customers ( 
   CustomerID INT PRIMARY KEY, 
   CustomerName VARCHAR(50), 
   ContactName VARCHAR(50), 
   Country VARCHAR(50) 
); 
INSERT INTO Customers (CustomerID, CustomerName, ContactName, Country) 
VALUES (1, 'ABC Company', 'John Smith', 'USA'), 
       (2, 'XYZ Corporation', 'Jane Doe', 'Canada'), 
       (3, 'PQR Inc', 'Bob Johnson', 'UK');     
```        
Bu kod parçası, "Customers" adında bir tablo oluşturur. Tablo, "CustomerID", "CustomerName", "ContactName" ve "Country" adlı sütunları içerir. "CustomerID" sütunu birincil anahtar olarak belirlenir, yani her satırın benzersiz bir "CustomerID" değeri olmalıdır. Daha sonra, "INSERT INTO" ifadesi kullanılarak tabloya üç satır eklendi. Bu satırlar, "CustomerID", "CustomerName", "ContactName" ve "Country" sütunlarına değerler atar.

Sonuç olarak, bu kod parçası, "Customers" adlı bir tablo oluşturur ve içine üç müşteri kaydı ekler.
