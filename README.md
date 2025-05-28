# E-commerce-Sales-Customer-Segmentation
## Proje Amacı

Bu projenin temel amacı, gerçek bir e-ticaret veri setini kullanarak kapsamlı bir **veri analizi** yapmak ve elde edilen bulgularla iş stratejilerini iyileştirmeye yönelik öneriler sunmaktır. Özellikle, **müşteri segmentasyonu** yaparak farklı müşteri gruplarının davranışlarını anlamak ve pazarlama kampanyalarını optimize etmek hedeflenmiştir. Bu proje, aşağıdaki yetenekleri sergilemek için tasarlanmıştır:

- **Veri Temizleme ve Ön İşleme:** Eksik değerlerin, aykırı değerlerin ve veri tutarsızlıklarının giderilmesi.
- **Keşifçi Veri Analizi (EDA):** Veri setindeki temel kalıpların, ilişkilerin ve anormalliklerin görselleştirme ve istatistiksel yöntemlerle belirlenmesi.
- **İş Zekası (BI) İçgörüleri:** Satış trendleri, en çok satan ürünler, gelir dağılımı gibi iş odaklı metriklerin analizi.
- **Müşteri Segmentasyonu:** RFM (Recency, Frequency, Monetary) analizi veya kümeleme algoritmaları (örneğin K-Means) kullanarak müşterileri anlamlı gruplara ayırma.
- **Öneriler ve İş Stratejileri:** Analiz sonuçlarına dayanarak pazarlama, ürün geliştirme ve operasyonel iyileştirmelere yönelik uygulanabilir öneriler sunma.

### Kullanılan Araçlar ve Teknolojiler

- **Programlama Dili:** Python
- **Kütüphaneler:**
    - **Veri Manipülasyonu:** `pandas`, `numpy`
    - **Veri Görselleştirme:** `matplotlib`, `seaborn`, `plotly` (interaktif görselleştirmeler için)
    - **Makine Öğrenimi (Segmentasyon için):** `scikit-learn` (K-Means vb.)
- **Ortam:** Jupyter Notebook
- **Versiyon Kontrolü:** Git & GitHub

### Veri Seti

Bu proje için Kaggle'dan veya benzeri bir kaynaktan halka açık bir e-ticaret veri seti kullanılacaktır. Örnek olarak, "Online Retail Data Set" veya "E-commerce Transactions" gibi veri setleri uygundur. Veri seti aşağıdaki sütunları içermelidir (veya benzeri):

- `InvoiceNo`: Fatura numarası
- `StockCode`: Ürün kodu
- `Description`: Ürün açıklaması
- `Quantity`: Satın alınan miktar
- `InvoiceDate`: Fatura tarihi
- `UnitPrice`: Birim fiyat
- `CustomerID`: Müşteri Kimliği
- `Country`: Ülke

[Online retail dataset](https://www.kaggle.com/datasets/lakshmi25npathi/online-retail-dataset?resource=download)

### Proje Akışı

1. **Veri Toplama ve Yükleme:** Seçilen e-ticaret veri setinin Jupyter Notebook ortamına aktarılması.
2. **Veri Temizleme ve Ön İşleme:**
    - Eksik değerlerin tespiti ve uygun yöntemlerle (silme, doldurma) ele alınması.
    - Aykırı değerlerin (outliers) tespiti ve yönetimi.
    - Veri tiplerinin kontrolü ve dönüştürülmesi (tarih formatları vb.).
    - Gereksiz sütunların veya yinelenen kayıtların belirlenmesi ve kaldırılması.
3. **Keşifçi Veri Analizi (EDA):**
    - Genel veri özeti (betimsel istatistikler).
    - Satışların zaman içindeki değişimi (günlük, haftalık, aylık trendler).
    - En çok satan ürünler ve kategoriler.
    - En çok gelir getiren müşteriler.
    - Ülkelere göre satış dağılımı.
    - Ortalama sipariş değeri ve sıklığı.
    - Korelasyon analizleri (varsa).
4. **RFM Analizi ve Müşteri Segmentasyonu:**
    - **Recency (Yenilik):** Müşterinin son alışverişinden bu yana geçen süre.
    - **Frequency (Sıklık):** Müşterinin toplam alışveriş sayısı.
    - **Monetary (Parasal Değer):** Müşterinin yaptığı toplam harcama.
    - RFM skorlarının hesaplanması ve müşterilerin segmentlere ayrılması (örn: "Sadık Müşteriler", "Riskli Müşteriler", "Yeni Müşteriler" vb.).
    - Gerekirse K-Means gibi kümeleme algoritmaları ile daha gelişmiş segmentasyon.
5. **Bulgular ve Öneriler:**
    - Her bir müşteri segmenti için ayrıntılı analiz ve davranışsal içgörüler.
    - Analiz sonuçlarına dayanarak iş stratejilerine yönelik somut, eyleme geçirilebilir öneriler (örn: kişiselleştirilmiş pazarlama kampanyaları, ürün önerileri, müşteri sadakat programları).
    - Görselleştirmelerle desteklenmiş özet rapor.

### Beklenen Çıktılar

- Temizlenmiş ve analiz için hazır veri seti.
- Kapsamlı EDA raporu ve görselleştirmeler.
- RFM veya kümeleme tabanlı müşteri segmentasyonunun sonuçları.
- Segmentlere özel iş stratejisi önerileri içeren bir sonuç bölümü.
- Proje kodunun, açıklayıcı yorumlarla birlikte düzenli bir Jupyter Notebook dosyası (`.ipynb`).
