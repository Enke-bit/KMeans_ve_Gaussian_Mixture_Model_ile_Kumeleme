# KMeans ve Gaussian Mixture Model ile Kümeleme
Bu kod, veri kümeleme yöntemlerini kullanarak verileri analiz etmeyi ve görselleştirmeyi amaçlamaktadır. İki farklı kümeleme algoritması olan KMeans ve Gaussian Mixture Model (GMM) kullanılarak verilerin nasıl kümelendiğini ve sonuçların nasıl görselleştirildiğini gösterir. İşte bu kodun temel bileşenleri ve işleyişi:

1. Veri Üretimi ve Hazırlığı
Veri Üretimi: İlk olarak, make_blobs fonksiyonu ile 400 örnek içeren, dört farklı merkez etrafında kümelenmiş yapay veri setleri üretilir. Bu veri seti, kümeleme algoritmalarının performansını değerlendirmek için kullanılır.
Veri Gerilmesi: Veriler üzerinde rastgele bir gerilme (stretching) işlemi uygulanır, bu da verilerin daha farklı bir dağılımda görselleştirilmesine olanak sağlar.
2. KMeans Kümeleme
KMeans Algoritması: KMeans algoritması, verileri belirli bir sayıda (bu örnekte 4) kümeye ayırır. Bu işlem, verilerin nasıl gruplandığını anlamak için kullanılır.
Küme Merkezleri: Algoritma sonuçları, her bir küme için merkez noktaları ile birlikte görselleştirilir. Küme merkezleri, kümelerin merkez noktalarını temsil eder ve genellikle büyük kırmızı noktalarla gösterilir.
3. Gaussian Mixture Model (GMM)
GMM Algoritması: GaussianMixture modeli, verileri çok sayıda (bu örnekte 4) Gauss dağılımı ile modellemeye çalışır. Bu, verilerdeki gizli yapıları daha esnek bir şekilde modellemek için kullanılır.
Elipsler ile Görselleştirme: Her bir Gauss bileşeni için, verilerin etrafında elipsler çizilir. Bu elipsler, her bileşenin kovaryansını ve ağırlığını temsil eder. Elipslerin büyüklüğü ve konumu, bileşenin veri üzerindeki etkisini görsel olarak gösterir.
4. Görselleştirme
KMeans ve GMM Sonuçları: Her iki algoritmanın sonuçları iki ayrı grafik üzerinde görselleştirilir:
Orijinal Veriler: İlk grafikte orijinal veri kümesi ve her bir algoritmanın küme merkezleri gösterilir.
Gerilmiş Veriler: İkinci grafikte, gerilmiş veri kümesi üzerinde algoritmaların nasıl çalıştığı ve sonuçların nasıl değiştiği gözlemlenir.
5. Kodun Yapısı ve Kullanımı
Fonksiyonlar: Kod, plot_kmeans, plot_gmm, ve draw_ellipse gibi fonksiyonlar içerir. Bu fonksiyonlar, kümeleri ve elipsleri çizmek için kullanılır ve kodun modülerliğini artırır.
Görselleştirme Ayarları: plt.subplots kullanılarak sonuçlar yan yana iki grafik olarak sunulur. Bu, verilerin ve algoritmaların karşılaştırılmasını kolaylaştırır.
Bu kod, KMeans ve GMM gibi kümeleme algoritmalarının nasıl çalıştığını ve verileri nasıl grupladığını anlamak için güçlü bir görselleştirme aracıdır. Görselleştirilen sonuçlar, algoritmaların farklı veri dağılımlarında nasıl performans gösterdiğini ve çeşitli kümeleme yöntemlerinin sonuçlarını nasıl etkilediğini anlamak için faydalıdır.
