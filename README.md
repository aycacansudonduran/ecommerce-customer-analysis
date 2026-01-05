# E-Ticaret Müşteri Analizi (RFM)

Bu proje, **Online Retail** veri seti kullanılarak müşteri satın alma davranışlarının analiz edilmesini amaçlamaktadır.  
Projenin temel hedefi, **RFM (Recency, Frequency, Monetary)** analizi ile müşteri segmentasyonu yapmak ve veri odaklı iş kararlarını desteklemektir.

---

## Proje Özeti

Müşteri davranışlarını anlamak, e-ticaret işletmeleri için kritik öneme sahiptir.  
Bu projede ham işlem verileri temizlenmiş, dönüştürülmüş ve analiz edilerek yüksek değerli, sadık ve risk altındaki müşteriler gibi anlamlı müşteri segmentleri oluşturulmuştur.

---

## Veri Seti

- **Kaynak:** Online Retail Veri Seti (Kaggle)
- **İçerik:** İşlem bazlı e-ticaret verileri
- **Dönem:** 2010–2011

> Ham veri dosyaları repoya eklenmemiştir ve `.gitignore` ile hariç tutulmuştur.

---

## Proje Yapısı

---

## 01 – Veri Temizleme

Bu adımda analiz için veri hazırlanmıştır:

- Eksik `CustomerID` değerleri kaldırıldı  
- İptal edilen işlemler (InvoiceNo “C” ile başlayanlar) çıkarıldı  
- Negatif miktar ve fiyat değerleri filtrelendi  
- Tarih alanları datetime formatına dönüştürüldü  
- `TotalPrice` değişkeni oluşturuldu  

---

## 02 – RFM Analizi

Müşteri bazlı RFM metrikleri hesaplanmıştır:

- **Recency:** Son alışverişten bu yana geçen gün sayısı  
- **Frequency:** Benzersiz işlem sayısı  
- **Monetary:** Toplam harcama tutarı  

RFM skorlarına göre müşteriler aşağıdaki segmentlere ayrılmıştır:
- Champions
- Loyal Customers
- Potential Loyalists
- At Risk
- Lost

---

## 03 – Keşifsel Veri Analizi (EDA)

Yapılan temel analizler ve görselleştirmeler:

- Segment bazlı müşteri sayısı  
- Segment bazlı toplam ciro  
- Segment bazlı ortalama sepet tutarı  
- Önemli segmentlerin karşılaştırılması (ör. Champions – At Risk)  

---

## Kullanılan Teknolojiler

- Python  
- Pandas  
- Matplotlib  
- Google Colab  

---

## Amaç

Bu projenin amacı, gerçek bir e-ticaret veri seti üzerinden veri temizleme, müşteri segmentasyonu ve keşifsel analiz becerilerini göstermektir.

---

## Yazar

Bu proje, veri bilimi portföyü amacıyla hazırlanmıştır.



