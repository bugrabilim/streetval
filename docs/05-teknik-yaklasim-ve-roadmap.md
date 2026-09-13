# Teknik Yaklaşım ve Yol Haritası

## Ürün Prensibi
StreetVal'in ilk sürümü, kişisel tanımlama veya takip yerine yalnızca toplulaştırılmış yoğunluk göstergelerine odaklanmalıdır. Teknik ve hukuki tasarımın başlangıç noktası veri minimizasyonu olmalıdır.

## Önerilen MVP

MVP'nin amacı doğrudan otomatik emlak fiyatı üretmek değil, şu hipotezi test etmektir:

> Mikro-lokasyon hareketlilik verisi, emlak profesyonellerinin değerleme veya yatırım kararlarında kullanmak isteyeceği anlamlı bir ek veri katmanı mıdır?

### MVP bileşenleri

1. Tek veya birkaç pilot lokasyon
2. Toplulaştırılmış yaya / araç yoğunluğu metriği
3. Saatlik ve günlük yoğunluk grafikleri
4. Lokasyon karşılaştırma ekranı
5. Basit bir StreetVal Location Score
6. CSV / rapor çıktısı
7. Emlak profesyonelleri için geri bildirim ekranı

## Önerilen Teknik Mimari

### Veri katmanı
- İzinli veri kaynaklarından toplulaştırılmış hareketlilik metrikleri
- Zaman damgası ve lokasyon etiketi
- Emlak / ilan / çevre verileri
- Veri kalite ve süreklilik kontrolleri

### Analitik katmanı
- Yoğunluk trendleri
- Saat / gün / hafta desenleri
- Lokasyonlar arası normalize karşılaştırma
- Anomali tespiti
- İlerleyen aşamada değerleme modellerine özellik olarak ekleme

### Ürün katmanı
- Web dashboard
- Harita tabanlı lokasyon görünümü
- API
- Raporlama

## Aşamalı Yol Haritası

### Faz 0: Problem doğrulama
- 15-30 emlak profesyoneli ile görüşme
- Hangi yoğunluk göstergelerine para ödeneceğini test etme
- Değerleme uzmanlarıyla veri anlamlılığını doğrulama
- Hukuki / gizlilik çerçevesini uzmanla netleştirme

### Faz 1: Teknik proof-of-concept
- Sınırlı lokasyon
- Toplulaştırılmış yaya ve araç yoğunluğu
- Veri kalite ölçümü
- Basit dashboard

### Faz 2: MVP
- Çoklu lokasyon
- Tarihsel trendler
- Lokasyon karşılaştırma
- StreetVal Location Score v1
- İlk ücretli pilot hedefi

### Faz 3: Veri ürünü
- API
- Kurumsal hesaplar
- Emlak platformu entegrasyonları
- Bölgesel kapsama genişlemesi

### Faz 4: Değerleme modeli
- Hareketlilik göstergelerinin fiyat / kira ile korelasyon analizi
- Bağımsız değerleme verileriyle model doğrulama
- Açıklanabilir karar destek modeli

## Başarı Metrikleri

- Pilot lokasyon sayısı
- Kesintisiz veri oranı
- Veri doğruluğu / sayım hata oranı
- Aktif kurumsal kullanıcı sayısı
- Ücretli pilot dönüşüm oranı
- API kullanım hacmi
- Müşteri başına aylık tekrar eden gelir
- Hareketlilik göstergelerinin değerleme doğruluğuna ölçülebilir katkısı

## Kritik İlke
StreetVal'in değer önerisi, "kameradan insan izleme" değil, **kişisel veri üretmeden lokasyon düzeyinde hareketlilik sinyali oluşturmak** olmalıdır. Ürünün teknik, hukuki ve ticari tasarımı bu sınırı korumalıdır.
