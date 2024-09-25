# Pusula_Esmanur _Alican
# esmnralicann@gmail.com 
# Pusula Data Science Case Study

## Proje Özeti

Bu proje, ilaç yan etkileriyle ilgili bir veri seti üzerinde çalışmayı içerir. Amaç, veri setini keşfetmek, eksik verileri işlemek ve daha sonra veri üzerinden çeşitli analizler yaparak modellemeye uygun hale getirmektir.

### Adımlar

1. **Keşifsel Veri Analizi (EDA)**:
   - Verinin genel yapısı analiz edildi.
   - Eksik değerler ve olası anomaliler tespit edildi.
   - Kategorik ve sayısal değişkenler arasındaki ilişkiler görselleştirildi.

2. **Veri Ön İşleme**:
   - Eksik değerler dolduruldu.
   - Kategorik veriler sayısal forma dönüştürüldü.
   - Normalizasyon ve standardizasyon işlemleri uygulandı.

3. **Veri Görselleştirme**:
   - Çeşitli görselleştirme teknikleri (histogram, scatter plot, ısı haritası) ile verinin dağılımları incelendi.
   - İlaçların yan etkileri ve demografik veriler arasındaki ilişkiler görselleştirildi.

### Dosya İçeriği

- **data**: Projede kullanılan ham veri setini içerir.
- **notebooks**: Jupyter Notebook dosyaları burada bulunur.
- **results**: İşlenen veriler ve analiz sonuçları burada bulunur.

### Kullanılan Kütüphaneler

- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

### Veri Ön İşleme Adımları

- **Eksik Verilerin Doldurulması**:
  - `Kilo` ve `Boy` sütunları medyan değerlerle dolduruldu.
  - Kategorik sütunlardaki eksik veriler mod ile dolduruldu.
  - İlaç başlangıç/bitiş tarihleri mantıksal yaklaşımlar kullanılarak dolduruldu.
  
- **Kategorik Verilerin Dönüştürülmesi**:
  - Cinsiyet, şehir ve ilaç adı gibi kategorik değişkenler OneHotEncoder veya LabelEncoder kullanılarak dönüştürüldü.

### Yapılan Analizler

1. **Yan Etkilerin Cinsiyet ve Yaş ile İlişkisi**:
   - Farklı cinsiyetlerin ve yaş gruplarının rapor ettiği yan etkiler analiz edildi.
   - Yaş ve yan etki arasındaki ilişki görselleştirildi.

2. **İlaç Kullanım Süresi ile Yan Etkiler**:
   - İlaç kullanım süresinin yan etkiler üzerindeki etkisi analiz edildi.

3. **Yan Etkilerin İstatistiksel Analizi**:
   - Her yan etki için istatistiksel dağılımlar çıkarıldı.
   - Tedavi süreleri ile yan etkiler arasında korelasyonlar tespit edildi.

### Hata Kontrolü ve İyileştirmeler

- Notebook dosyasının başında veri yüklenirken `NaN` değerlerinin doğru şekilde ele alındığından emin olundu.
- Eksik değerlerin doldurulması sırasında veri tipi uyuşmazlıkları olup olmadığı kontrol edildi.
- Görselleştirme aşamasında eksik veri veya anlamsız sonuçlar olmadığından emin olundu.

### Sonuçlar

- Yan etkilerin raporlanma olasılığı demografik verilere göre değişiklik gösterdi.
- Belirli ilaçların kullanım süresi arttıkça yan etkilerdeki artış gözlemlendi.
- Bu veriler, ilaç güvenliği ve kişiselleştirilmiş tedavi stratejileri geliştirmek için kullanılabilir.

