# Ara Rapor - ESP32 Tabanlı Web Arayüzlü Akıllı Sulama Sistemi

## 1. Proje Konusu
Toprak nemine duyarlı, Wi-Fi üzerinden uzaktan erişilebilen ve otomatik sulama yapabilen, ESP32 tabanlı akıllı tarım sistemi geliştirilmesi.

## 2. Özet
Bu proje kapsamında, ESP32 mikrodenetleyici kullanılarak toprak nemini ölçen ve kullanıcıya internet üzerinden bu veriyi sunan bir sistem geliştirilmiştir. Sistem, nem seviyesi belirli bir eşik değerin altına düştüğünde otomatik olarak sulama başlatmakta, web arayüzü üzerinden izleme ve kontrol imkanı sunmaktadır. Sistem modüler tasarlanmış olup, ileride farklı bitki türlerine özel sulama eşikleri belirlenmesi ve gömülü sistemin 3D baskı ile tek bir muhafazada birleştirilmesi hedeflenmektedir. Ticari anlamda düşük maliyetli, ölçeklenebilir bir çözüm sunmayı amaçlamaktadır.

## 3. Kullanılan Yöntemler
- *Mikrodenetleyici:* ESP32 Wi-Fi destekli mikrodenetleyici.
- *Programlama Dili:* C++ (Arduino IDE), HTML & CSS (Web Arayüzü).
- *Sunucu:* ESP32 üzerinde çalışan yerel HTTP sunucusu.
- *Web Arayüzü:* HTML tabanlı, gerçek zamanlı veri sunumu sağlayan hafif arayüz.
- *Kontrol Algoritması:* ADC üzerinden nem ölçümü, eşik karşılaştırması, servo tetiklemesi.
- *Gelecek Planı:* REST API ile bitki türüne özgü eşik değerlerinin belirlenmesi.
## 4. Yapılan Çalışmalar ve Görselleri
- ESP32 mikrodenetleyici üzerinde çalışan web sunucusu oluşturuldu.
- Toprak nem sensöründen gelen analog veri dijital ortama aktarıldı ve normalize edildi.
- Servo motor, nem eşik değerine göre tetiklendi.
- HTML ve CSS kullanılarak görsel bir arayüz oluşturuldu.
- Web arayüzü üzerinden anlık nem değeri takibi sağlandı.
- Donanım ve yazılım kısmı ayrı modüller halinde geliştirildi.

📷 Görseller:
- Cihazın genel görünümü:
  ![image](https://github.com/cpnertugrul/plant-irrigation-IoT-project/blob/araRapor/Figure/proje_gorsel_prototip.jpg)
- Web arayüz ekran görüntüsü:
  ![image](https://github.com/cpnertugrul/plant-irrigation-IoT-project/blob/araRapor/Figure/proje_gorsel_arayuz.jpg)


## 5. Elde Edilen Sonuçlar
- Sistemin temel işlevleri başarıyla gerçekleştirildi.
- Web arayüzü üzerinden gerçek zamanlı toprak nemi takibi yapılabilmektedir.
- Nem seviyesi eşik değerinin altına düştüğünde otomatik sulama tetiklenmektedir.
- Kod yapısı modüler olarak tasarlanmıştır, bu sayede farklı bitki türleri için özelleştirme yapılabilir hale gelmiştir.
## 6. Karşılaşılan Sorunlar ve Çözümler
| Karşılaşılan Zorluk | Getirilen Çözüm |
|---------------------|------------------|
| Nem sensöründen gelen verilerin kararsız olması | Ortalama alma ve düşük geçiren filtre uygulanarak veri kararlılığı sağlandı. |
| Servo motorun stabil çalışmaması | Kod içinde PWM sinyal süreleri optimize edildi. |
| Web sunucusuna erişim sorunları | ESP32 için sabit IP atanarak bağlantı problemleri giderildi. |

## 7. Projenin Devamında Yapılacaklar
- REST API entegrasyonu ile farklı bitki türlerine göre ideal nem seviyelerinin çekilmesi ve eşik değerlerin dinamik olarak belirlenmesi.
- Manuel kontrol butonlarının web arayüzüne eklenmesi.
- 3D yazıcı ile fiziksel donanımın birleştirilerek kompakt hale getirilmesi.
- Projenin ürünleştirilmesi ve küçük ölçekli bir prototip üretimi için pazar analizi yapılması.
