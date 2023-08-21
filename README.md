<img src="https://github.com/TRA-Tech/sql-sqlserver/assets/100773960/0ef9b179-8bdb-47f0-a8a5-765c696b9606" width="75" height="75"> 


# SQL
SQL (Structured Query Language), ilişkisel veritabanı yönetim sistemlerinde kullanılan bir programlama dilidir. SQL, veritabanlarında veri eklemek, güncellemek, silmek ve sorgulamak için kullanılır.

SQL, 1970'lerde IBM tarafından geliştirilmiş ve daha sonra ANSI (American National Standards Institute) ve ISO (International Organization for Standardization) tarafından standartlaştırılmıştır. SQL, ilişkisel veritabanı yönetim sistemleri (RDBMS) için özellikle tasarlanmıştır ve birçok RDBMS, özellikle Oracle, MySQL, MSSQL, PostgreSQL ve SQLite tarafından desteklenir.

SQL, basit ve kolay anlaşılır bir dil olması nedeniyle çok yaygın olarak kullanılır. SQL sorguları, veritabanlarına erişmek için kullanılan birçok uygulamada kullanılabilir. SQL, veritabanlarında veri işleme işlemlerini otomatikleştirmeye ve hızlandırmaya yardımcı olan birçok özellik ve fonksiyona sahiptir. SQL sorguları, veritabanı işlemlerini gerçekleştirmek için tasarlanmıştır ve sorguların sonuçları, veritabanında depolanan verilerin bir görüntüsünü oluşturur.
<br>
<br>
Veritabanı yaklaşımı ile birlikte bir veri sorgulama diline veya aracına ihtiyaç duyulmuştur. İlk başta matematiksel bir sözdizimine sahip olan SQUARE adlı bir dil geliştirilmiştir. Geniş kullanıcı kitleleri tarafında kolay kullanılabilmesi için matematiksel söz dizimli SQUARE dilinden vazgeçilerek, İngilizceye benzer sözdizimine sahip bir dil oluşturulmuş ve SEQUEL olarak adlandırılmıştır. Daha sonra da bu SEQUEL dili, İngilizce söylenişine paralel olarak SQL olarak adlandırılmıştır.

SQL dili ilişkisel alanda büyük ilgi görmüş ve İlişkisel Veri Tabanı Yönetim Sistemlerinin (İVTYS) tümünde yer alan standart dil görünümü kazanmıştır. Bu nedenle Veri Tabanı konusunda çalışan tüm bilişim teknik personeli tarafından bilinmesi gereken bir dil konumundadır.
<br>

Kısaca bilinmesi gereken terimler de aşağıdaki gibidir.

- **Veritabanı:** MSSQL'de verilerin depolandığı ana yapıdır. Veritabanı, bir veya daha fazla tablodan oluşabilir ve kullanıcılar verileri burada saklarlar.
- **Tablo:** Verilerin belirli bir şekilde sıralandığı yapıdır. Tablolar, sütunlar ve satırlar içerir ve her satır, tablonun belirli bir sütunundaki verileri içerir.
- **Sütun:** Tablolarda depolanan verilerin belirli bir türde depolandığı yapıdır. Örneğin, bir müşteri tablosunda sütunlar adı, soyadı, adresi, telefon numarası gibi bilgileri içerebilir.
- **Satır:** Tablolarda depolanan verilerin her bir öğesi satır olarak adlandırılır. Örneğin, müşteri tablosunda bir satır, bir müşterinin adını, soyadını, adresini ve telefon numarasını içerebilir.
- **Sorgu:** Veritabanında belirli verileri bulmak veya değiştirmek için kullanılan bir işlemdir. Sorgular SQL dilinde yazılır ve belirli bir veritabanı işlemi gerçekleştirmek için kullanılır. Örneğin, müşterilerin adreslerini aramak için bir sorgu yazılabilir.
- **İndex:** Bir tablonun performansını artırmak için kullanılan bir yapıdır. İndexler, belirli bir sütuna göre sıralama yaparak sorgu işlemlerinin daha hızlı çalışmasına yardımcı olabilir.
- **Depolama Prosedürü:** Veritabanında depolanan işlevleri ifade eder. Depolama prosedürleri, verileri aramak, ekleme veya güncelleme gibi belirli bir veritabanı işlemi gerçekleştirmek için kullanılabilir.
- **Yedekleme:** Veritabanının yedeklenmesi ve kurtarılması işlemidir. Veritabanının yedeklenmesi, veri kaybını önlemek için önemlidir. Yedekler, bir veritabanı felaket durumunda kullanılabilir.
- **Yapılandırma Yöneticisi:** MSSQL sunucusunun yapılandırılmasını sağlar. Yapılandırma yöneticisi, sunucu ayarlarını değiştirme, kullanıcı hesaplarını yönetme ve veritabanı erişim izinlerini ayarlama gibi görevleri yapabilir.
- **Bağlantı Dizesi:** MSSQL sunucusuna bağlanmak için gereken bilgileri içerir. Bağlantı dizesi, veritabanı adı, sunucu adı, kullanıcı adı ve şifre gibi bilgileri içerir ve MSSQL sunucusuna erişmek için kullanılır.

## SQL dilini kullanan veritabanları
- Microsoft SQL Server
- Sybase 
- MySQL
- PostgreSQL
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

  
![image](https://github.com/TRA-Tech/sql-sqlserver/assets/100773960/b3635941-55c7-4b7f-b2ab-b7931f660982)


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


# SQL Server
![image](https://github.com/TRA-Tech/sql-sqlserver/assets/100773960/0e6582a0-80e6-417d-82a5-51e6d0ed6193)

SQL Server, Microsoft tarafından geliştirilen bir ilişkisel veritabanı yönetim sistemidir. Veritabanı yönetim sistemleri (DBMS), verileri düzenlemek, depolamak ve yönetmek için kullanılan yazılım araçlarıdır. SQL Server, büyük işletmelerden küçük ölçekli projelere kadar çeşitli kullanım durumlarına uygun olarak tasarlanmıştır.

## Temel Özellikleri

- **Veri Depolama ve Yönetim** :
SQL Server, yapılandırılmış veri depolama imkanı sunar. Veriler tablolarda düzenlenir ve SQL (Structured Query Language) kullanılarak sorgulanır. Bu sayede veri güvenliği, bütünlük ve erişilebilirlik sağlanır.


- **Güvenlik** :
SQL Server, veritabanı güvenliği için çeşitli mekanizmalar sunar. Kullanıcı ve roller yönetimi, veri şifreleme, izin ayarları gibi özelliklerle verilerin korunması sağlanır.


- **Yedekleme ve Kurtarma** :
Veri kaybını önlemek için SQL Server yedekleme ve kurtarma özellikleri sunar. Verilerin düzenli olarak yedeklenmesi ve gerektiğinde geri yüklenmesi sağlanır.


- **Yüksek Erişilebilirlik** :
SQL Server, yüksek erişilebilirlik sağlamak için çeşitli özellikler sunar. Failover Cluster Instance (FCI) ve Always On Availability Groups gibi yöntemlerle kesintisiz hizmet sağlanır.


- **Veritabanı Uygulama Geliştirme** :
SQL Server, veritabanı uygulamaları geliştirmek için geniş bir araç ve dil yelpazesi sunar. Stored procedure'ler, view'lar ve iş tetikleyiciler gibi özelliklerle veritabanı mantığı kod tarafında uygulanabilir.


- **İş Zekası ve Raporlama** :
SQL Server, verilerin analiz edilmesi ve raporlanması için Business Intelligence (BI) araçları sunar. Integration Services (SSIS), Analysis Services (SSAS) ve Reporting Services (SSRS) gibi bileşenlerle verilerin işlenmesi ve görselleştirilmesi sağlanır.


- **Sürümler ve Lisanslama** :
SQL Server, farklı sürümler halinde gelir ve bu sürümler farklı özelliklere ve kullanım durumlarına yönelik tasarlanmıştır. Lisanslama da bu sürümlere göre değişiklik gösterebilir.


Sonuç olarak SQL Server, veritabanı yönetimi ve iş zekası ihtiyaçlarını karşılamak için geniş bir yelpazede özellik sunan güçlü bir DBMS'dir. Veri yönetimi, güvenlik, yedekleme, geliştirme ve raporlama gibi çeşitli alanlarda kullanılabilecek esneklik sunar.

