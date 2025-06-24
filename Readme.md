# 🛫 Airline Passenger Satisfaction Analysis

Bu proje, Patika Kız Başına Veri Analizi Bootcampi kapsamında gerçekleştirilmiş olup, Airline Passenger Satisfaction Dataset üzerinde veri analizi çalışmasını içermektedir.

## 🎯 Amaç

Projenin amacı, havayolu yolcularının memnuniyet düzeylerini etkileyen faktörleri belirlemek; istatistiksel özetler, eksik değer analizi, aykırı değer tespiti ve uygun görselleştirmelerle desteklenen bir analiz gerçekleştirmektir.

## 📁 Veri Seti

- **Veri Seti:** Airline Passenger Satisfaction Dataset  
- **Satır Sayısı:** 103.904  
- **Değişken Sayısı:** 25  
- **Hedef Değişken:** `satisfaction` (`satisfied` / `neutral or dissatisfied`)

## 🔍 Analiz Süreci

### 1. Veri Ön İşleme
- Veri tipleri kontrol edilip uygun biçimlendirildi.

### 2. İstatistiksel Özet
- Tüm sayısal değişkenler için ortalama, medyan, min, max, standart sapma gibi özetler çıkarıldı ve yorumlandı.

### 3. Eksik Değer Analizi
- Yalnızca `Arrival Delay in Minutes` sütununda %0.29 oranında eksik değer bulundu.
- Verinin dağılımı sağa çarpık olduğu için medyan ile doldurma yöntemi tercih edildi.

### 4. Aykırı Değer Tespiti
- IQR yöntemiyle tüm sayısal değişkenlerde aykırı değer analizi yapıldı.
- `Flight Distance`, `Checkin Service`, `Departure Delay`, `Arrival Delay` değişkenlerinde yüksek sayıda aykırı değer bulundu.
- Boxplot ile görsel destek sağlandı.

### 5. Görselleştirme
- Veriyi daha iyi anlamak ve içgörü elde etmek amacıyla hem sayısal hem de kategorik değişkenler için çeşitli grafikler kullanılmıştır.

## 📈 Öne Çıkan Bulgular

- **Loyal Customers** memnuniyet açısından daha önde.
- **Business Class** yolcuları en yüksek memnuniyet düzeyine sahipken, **Eco** sınıfı yolcular genellikle memnun değil.
- **Wi-Fi hizmeti** tüm yolcular için en düşük puanlanan hizmet.
- **Yaş gruplarında** memnuniyet 36-50 yaş grubunda zirvedeyken, 0-13 ve 66+ yaş gruplarında düşüktür.
- **Uzun uçuşlar**, kısa uçuşlara kıyasla daha yüksek memnuniyet oranına sahiptir.

## 💼 Kullanılan Araçlar

- Python
- Pandas, NumPy
- Seaborn, Matplotlib
- Jupyter Notebook

## 📂 Proje Yapısı

```bash
├── notebooks 
   ├── airline_analysis.ipynb     # Ana analiz dosyası
├── README.md                  # Bu açıklama dosyası
└── data/                   # (Opsiyonel) Veri setinin bulunduğu klasör
