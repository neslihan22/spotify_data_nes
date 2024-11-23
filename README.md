
https://www.kaggle.com/code/neslihantoprak/spotify-data-analiz-neslihantoprak/edit/run/209170555

ya da spotify-data-analiz-neslihantoprak.ipynb ile ulaşabilirsiniz.


SPOTİFY VERi ANALİZ
Kullanılan kütüphaneler:

Pandas, veri işleme ve analizi için kullanılan güçlü bir Python kütüphanesidir. Özellikle CSV dosyalarından veri yüklemek, veri çerçeveleri (DataFrames) ile çalışmak ve veriyi manipüle etmek için kullanılır.

Matplotlib, 2D grafikler ve görselleştirmeler oluşturmak için kullanılan bir kütüphanedir. Verilerin görselleştirilmesi için çizgi grafikler, çubuk grafikler, histogramlar ve daha fazlasını oluşturabiliriz.

Kullanım: Verileri görselleştirmek, çizgi grafikleri, histogramlar ve diğer görsel analizleri oluşturmak.


Seaborn, Matplotlib üzerine inşa edilmiş ve veri görselleştirmelerini daha estetik hale getiren bir kütüphanedir. Veri çerçeveleri ile uyumlu çalışır ve gelişmiş görselleştirmeler sunar.

Kullanım: İleri düzey görselleştirmeler, korelasyon haritaları, dağılım grafiklerine estetik eklemek.


os kütüphanesi, dosya ve dizin işlemleri yapmanızı sağlar. Dosya yollarını yönetme, dosya okuma/yazma ve dizin içinde gezinme gibi işlemler için kullanılır.

Kullanım: Dosya yollarını kontrol etmek, dosya ve klasör işlemleri yapmak.


random kütüphanesi, rastgele sayılar üretmek, rastgele seçimler yapmak ve benzeri işlemler için kullanılır.

Kullanım: Veri seti üzerinde rastgele işlemler yapmak, örnekleme, karıştırma.


missingno kütüphanesi, eksik veri tespiti ve görselleştirmesi yapmak için kullanılır. Veri setindeki eksik değerlerin görsel olarak incelenmesine olanak tanır.

Kullanım: Eksik verilerin analizi ve görselleştirilmesi, eksik veri durumunu hızlıca tespit etmek.
track_id: Her bir şarkının benzersiz kimliği.
artists: Şarkıyı seslendiren sanatçılar.
album_name: Şarkının yer aldığı albüm.
track_name: Şarkının adı.
popularity: Şarkının popülerlik seviyesi (0-100 arasında bir değer).
duration_ms: Şarkının uzunluğu (milisaniye cinsinden).
explicit: Şarkının açık içerik (explicit) içerip içermediğini belirten Boolean değer (False/True).
danceability: Şarkının dans edilebilirlik seviyesi (0 ile 1 arasında).
energy: Şarkının enerjik olma seviyesi (0 ile 1 arasında).
key: Müzikal tonun hangi nota üzerinde olduğu.
loudness: Şarkının ses şiddeti.
acousticness: Şarkının akustik özelliklerinin seviyesi (0 ile 1 arasında).
instrumentalness: Şarkının enstrümantal olma oranı.
liveness: Şarkının canlılık seviyesi.
valence: Şarkının genel ruh halini ifade eder; pozitif ruh hali 0 ile 1 arasında değişir.
tempo: Şarkının temposu (dakika başına vurgu sayısı).
time_signature: Şarkının zaman ölçüsü.
track_genre: Şarkının türü.
duration_range: Şarkının süresi ile ilgili kategorik bilgi (örneğin, "Short", "Medium").
continent: (Eklediğimiz bir sütun) Şarkının türüne göre kıta tahmini (örneğin, "North America", "Europe").


Bu bilgilerden sonra veri analizi aşamaları şöyledir:
1.VERİ SETİNİN HAZIRLANMASI
2.VERİYE İLK BAKIŞ
3.EKSİK VERİ ANALİZİ
4.KATEGORİK DEĞİŞKEN ANALİZİ
5.SÜREKLİ DEĞİŞKEN ANALİZİ
6.AYKIRI DEĞER ANALİZİ
7.FEATURE ENGİNEERİNG



En çok tercih edilen türler, ülkelerin dinlenmeleri en fazla hangi ülkelerden oluşan bir veriseti olduğunu görüyoruz.UK,JAPAN, USA ülkeleri fazlasıyla var.Tercih edilen türler ile ilgili notlar kodda mevcuttur.Aykırı değerler için çeşitli yöntemlerle düzeltmeler yapılmıştır.
Müzik türlerine göre kıta tahmini yapan fonksiyon yazarak veriyi tahminle bitiriyoruz.


