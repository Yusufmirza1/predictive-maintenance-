Predictive Maintenance Projesi
Bu proje, makine operasyonlarına ilişkin verileri analiz ederek ve modelleyerek, tahmini bakım süreçlerine odaklanmaktadır. Amacımız, çeşitli operasyonel parametrelere dayanarak makine arızalarını önceden tahmin etmektir. Bu projede, Rastgele Orman (Random Forest) algoritması kullanılarak bir sınıflandırma modeli oluşturulmuştur.

Proje Özeti
1. Verinin Yüklenmesi ve İlk İnceleme
Amaç: Veri setini yüklemek ve veri yapısını genel olarak anlamak.
Adımlar:
Veriyi pandas kullanarak yüklemek.
İlk birkaç satırı, veri türlerini görüntülemek ve eksik verileri kontrol etmek.
Sayısal sütunlar için temel istatistiksel özetler oluşturmak.
2. Veri Görselleştirme
Amaç: Önemli sayısal özelliklerin dağılımlarını görselleştirerek, belirli kalıpları veya anormallikleri tespit etmek.
Adımlar:
Air temperature [K] ve Process temperature [K] sütunlarının histogramlarını ve yoğunluk eğrilerini oluşturmak.
Veriler arasındaki ilişkileri incelemek için korelasyon matrisi oluşturmak.
3. Yeni Özellik Oluşturma
Amaç: Mevcut verilerden anlamlı bir özellik yaratmak.
Adım:
Process temperature [K] ile Air temperature [K] arasındaki farkı hesaplayarak yeni bir Temperature Difference sütunu eklemek.
4. Hedef Değişkenin Dağılımını İnceleme
Amaç: Hedef değişken olan Machine failure sınıfının dağılımını anlamak.
Adım:
Machine failure sütunu için bir sayım grafiği oluşturmak.
5. Kategorik Değişkenlerin Sayısallaştırılması
Amaç: Kategorik verileri sayısal forma dönüştürmek.
Adım:
Type sütununu one-hot encoding yöntemiyle sayısallaştırmak.
6. Modelin Eğitimi ve Değerlendirilmesi
Amaç: Veri setini eğitim ve test setlerine bölerek modeli eğitmek ve model performansını değerlendirmek.
Adımlar:
Veriyi %80 eğitim, %20 test olacak şekilde bölmek.
Rastgele Orman algoritması ile modeli eğitmek ve test seti üzerinde tahmin yapmak.
Model performansını değerlendirmek için karışıklık matrisi ve sınıflandırma raporu oluşturmak.
7. Özellik Önem Düzeylerinin Görselleştirilmesi
Amaç: Modelin hangi özelliklere ne kadar önem verdiğini anlamak.
Adım:
Modelin atfettiği önem düzeylerini bar grafiği olarak görselleştirmek.
