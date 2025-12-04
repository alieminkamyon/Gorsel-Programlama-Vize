# Gorsel-Programlama-Vize

Bu proje, Türkiye'deki resmi tatil günlerini halka açık bir API üzerinden dinamik olarak çeken ve kullanıcıya konsol ekranı üzerinden çeşitli filtreleme/arama seçenekleri sunan bir C# .NET uygulamasıdır.


Uygulama, internet üzerinden güncel tatil verilerini asenkron olarak çeker ve kullanıcı dostu bir menü ile bu veriler üzerinde işlem yapılmasına olanak tanır. Veri manipülasyonu ve sorgulama işlemleri için modern C# teknikleri kullanılmıştır.


Kullanıcı, konsol ekranında aşağıdaki işlemlerden birini seçebilir:

Yıla Göre Listeleme: Kullanıcının girdiği belirli bir yıla (Örn: 2024) ait tüm resmi tatilleri listeler.

Tarihe Göre Arama: Belirli bir tarihte (Gün/Ay/Yıl) tatil olup olmadığını kontrol eder.

İsme Göre Arama: Tatil ismine göre (Örn: "Cumhuriyet") arama yapar ve eşleşen sonuçları getirir.

3 Yıllık Geniş Liste: Bulunulan yıl ve sonraki 2 yılı kapsayan tüm tatil listesini görüntüler.


Bu proje geliştirilirken aşağıdaki C# kütüphaneleri ve programlama konseptleri kullanılmıştır:

HttpClient: Harici bir REST API'ye bağlanarak tatil verilerini (GET isteği ile) internetten çekmek için kullanılmıştır.

System.Text.Json: API'den dönen JSON formatındaki veriyi, uygulama içerisinde kullanılabilir C# nesnelerine (Deserialize) dönüştürmek için kullanılmıştır.

Async / Await: Ağ işlemleri sırasında uygulamanın donmasını engellemek ve verileri asenkron (eşzamansız) olarak çekmek için tercih edilmiştir.

LINQ (Language Integrated Query): Çekilen tatil listesi üzerinde filtreleme (Where), sıralama (OrderBy) ve seçim (Select) işlemleri yapmak için kullanılmıştır.
