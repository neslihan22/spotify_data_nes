SPOTİFY VER ANALİZ
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

Pandas: Veri yapıları ve veri analizi için kullanılır.
Seaborn: Verilerin görselleştirilmesi için kullanılır.
Matplotlib: Verilerin görselleştirilmesi için kullanılır (Seaborn Matplotlib üzerine inşa edilmiştir).


En çok tercih edilen türler, ülkelerin dinlenmeleri en fazla hangi ülkelerden oluşan bir veriseti olduğunu görüyoruz.UK,JAPAN, USA ülkeleri fazlasıyla var.Tercih edilen türler ile ilgili notlar kodda mevcuttur.Aykırı değerler için çeşitli yöntemlerle düzeltmeler yapılmıştır.
Müzik türlerine göre kıta tahmini yapan fonksiyon yazarak veriyi tahminle bitiriyoruz.


