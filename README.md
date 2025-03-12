# 🌱 plant-irrigation-IoT-project

Bu proje, ESP32 mikrodenetleyicisi kullanarak bitkilerin toprak nem seviyesine göre otomatik olarak sulanmasını sağlayan bir IoT tabanlı sistemdir. Sistem, bir toprak nem sensörü aracılığıyla verileri alır, belirlenen eşik değerinin altına düştüğünde su pompasını çalıştırır ve aynı zamanda verileri bir IoT platformuna (örneğin Firebase, MQTT, Blynk) gönderir.  

## 🚀 Proje Özeti  
Bitkilerin sağlıklı büyümesini sağlamak için otomatik sulama sistemleri büyük kolaylık sağlar. Bu projede, ESP32 WiFi modülü sayesinde sensör verileri uzaktan takip edilebilir ve sulama işlemi manuel olarak da başlatılabilir.  

## 📌 Özellikler  
✅ *Otomatik Sulama*: Toprak nem sensöründen gelen veriye göre su pompasını açıp kapatma  
✅ *IoT Entegrasyonu*: Nem verilerini gerçek zamanlı olarak bir mobil uygulama veya web panelinde görüntüleme  
✅ *Uzaktan Kontrol*: Kullanıcı, internet üzerinden sulamayı manuel olarak başlatabilir veya zamanlayabilir  
✅ *Enerji Verimliliği*: Sistem düşük güç tüketimiyle çalışacak şekilde optimize edilmiştir  

## 🛠 Kullanılan Bileşenler  
- *ESP32* → WiFi ve Bluetooth desteği olan mikrodenetleyici  
- *Toprak Nem Sensörü* → Kapasitif nem sensörü tercih edilir (daha stabil)  
- *Su Pompası veya Selenoid Vana* → Sulama işlemi için kontrol edilir  
- *Röle Modülü* → Pompayı veya vanayı ESP32 üzerinden açıp kapamak için kullanılır  
- *Güç Kaynağı* → 5V veya 12V (kullanılan pompa/valfe bağlı olarak değişir)  

## 📡 IoT Entegrasyonu  
Bu proje için veriler aşağıdaki platformlardan biri kullanılarak uzaktan izlenebilir ve kontrol edilebilir:  
- *Blynk* (Mobil uygulama desteği ile kolay kontrol)  
- *Firebase Realtime Database* (Gerçek zamanlı veri takibi)  
- *MQTT* (IoT cihazlar arasında hızlı veri alışverişi)  

## 🔧 Çalışma Mantığı  
1. ESP32, toprak nem sensöründen veri okur.  
2. Nem seviyesi belirlenen eşiğin altına düştüğünde su pompası çalıştırılır.  
3. Sensör verileri belirlenen IoT platformuna gönderilir.  
4. Kullanıcı, mobil uygulama veya web paneli üzerinden durumu takip edebilir ve gerektiğinde sulamayı manuel olarak başlatabilir.  

## 📄 Lisans  
Bu proje açık kaynaklıdır, geliştirip paylaşabilir
siniz.
