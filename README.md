# 🌐 Yönlendirme Protokollerinde En Kısa Yol Optimizasyonu

[cite_start]Bu proje, bilgisayar ağlarında veri paketlerinin yönlendirilmesi (routing) sırasında karşılaşılan trafik sıkışıklığı ve darboğaz problemlerini analiz etmek üzere geliştirilmiş kapsamlı bir ağ simülasyonu ve algoritma tasarımı çalışmasıdır[cite: 7]. [cite_start]Proje kapsamında, geleneksel Dijkstra ve Bellman-Ford algoritmalarının dinamik ağ koşullarındaki yetersizlikleri incelenmiş ve bu soruna çözüm olarak "Trafik Duyarlı Dinamik Yönlendirme Algoritması" geliştirilmiştir[cite: 8, 9].

## 🚀 Proje Özeti ve Amacı
[cite_start]Geleneksel yönlendirme algoritmaları genellikle sadece fiziksel mesafeye veya bant genişliğine odaklanan "kör" bir yapıya sahiptir[cite: 12]. [cite_start]Bu proje, "en kısa yolun" her zaman "en hızlı" veya "en verimli" yol olmadığı hipotezini kanıtlamayı ve mühendislik tabanlı bir çözüm üretmeyi amaçlar[cite: 13].

* [cite_start]**Dinamik Maliyet Fonksiyonu:** Anlık hat doluluk oranlarını bir ceza katsayısı ile maliyet fonksiyonuna dahil eder[cite: 14].
* [cite_start]**Optimizasyon:** Veri trafiğini yoğun hatlardan uzaklaştırarak daha uzun ancak daha akıcı alternatif rotalara yönlendirir[cite: 14].
* [cite_start]**Analiz:** Algoritmaları işlemci süresi, zaman karmaşıklığı ve rota verimliliği açısından kıyaslar[cite: 17].

## 🛠️ Teknik Özellikler ve Metot
* [cite_start]**Dil:** Python [cite: 9]
* [cite_start]**Kütüphaneler:** `NetworkX` (Çizge teorisi), `Matplotlib` (Görselleştirme), `heapq` (Öncelik kuyruğu optimizasyonu)[cite: 43, 44].
* [cite_start]**Topoloji:** 50 adet yönlendirici düğümden oluşan "Rastgele Geometrik Çizge" modeli kullanılmıştır[cite: 47, 49].
* [cite_start]**Maliyet Formülü:** $Maliyet = Mesafe \times (1 + (Trafik \: Yoğunluğu \times Ceza \: Katsayısı))$[cite: 16].

---

## 📊 Algoritma Karşılaştırmaları

### 1. İşlemci Performansı
[cite_start]Düğüm sayısı arttıkça Bellman-Ford algoritması çizgisel olmayan bir süre artışı sergilerken, geliştirilen Trafik Duyarlı algoritma Klasik Dijkstra ile benzer şekilde yüksek ölçeklenebilirlik sunar[cite: 78, 79].

> **[GÖRSEL YERİ: Şekil 3 - 3 Algoritmanın Performans Karşılaştırma Grafiği]**

### 2. Adım Sayısı Verimliliği
[cite_start]Dijkstra tabanlı yaklaşım, aynı en kısa yolu bulurken Bellman-Ford'a göre yaklaşık 3.5 kat daha az işlem adımı gerçekleştirerek işlemci yükünü minimize eder[cite: 84, 85].

> **[GÖRSEL YERİ: Şekil 4 - Bellman Ford ve Dijkstra Görsel Karşılaştırma]**

### 3. Trafik Farkındalığı
Standart Dijkstra, %95 doluluk oranına sahip kısa yolu seçip darboğaza girerken; [cite_start]Geliştirilmiş Algoritma, trafiği tespit ederek daha uzun ama akıcı olan rotayı tercih eder[cite: 89, 90, 91].

> **[GÖRSEL YERİ: Şekil 5 - Standart ve Trafik Duyarlı Yönlendirme Karşılaştırması]**

---

## 📸 Simülasyon Arayüzü
[cite_start]Geliştirilen yazılım, 50 düğümlü ağ üzerindeki hatları trafik yoğunluğuna göre dinamik olarak renklendirir (Yeşil: Rahat, Kırmızı: Kritik Yoğunluk)[cite: 94, 95, 96].

> **[GÖRSEL YERİ: Şekil 7 - 50 Router ile Akıllı Ağ Simülasyonu Sonuç Ekranı]**

## 👥 Geliştiriciler
* [cite_start]**Özgür Taşkıran** - 23181616016 [cite: 3]
* [cite_start]**Ömer Faruk Aşkın** - 23181616758 [cite: 4]

---
[cite_start]*Bu çalışma, Gazi Üniversitesi Teknoloji Fakültesi Bilgisayar Mühendisliği Bölümü BMT-317 Algoritmalar dersi dönem sonu projesi kapsamında hazırlanmıştır[cite: 1, 2].*
