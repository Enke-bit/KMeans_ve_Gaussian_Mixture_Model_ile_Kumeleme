# KMeans ve Gaussian Mixture Model ile Veri Kümeleme
Bu proje, KMeans ve Gaussian Mixture Model (GMM) algoritmalarını kullanarak veri kümeleme yöntemlerini anlamak ve sonuçları görselleştirmek amacıyla geliştirilmiştir. Proje, çeşitli veri kümeleme tekniklerinin nasıl çalıştığını ve bu tekniklerin farklı veri dağılımlarında nasıl performans gösterdiğini incelemektedir.

## İçerik
- Veri Üretimi ve Hazırlığı
- KMeans Kümeleme
- Gaussian Mixture Model (GMM)
- Görselleştirme
- Kodun Yapısı ve Kullanımı
## Kurulum
Bu projeyi çalıştırmak için aşağıdaki adımları izleyebilirsiniz:

## Gerekli Kütüphaneler:

Proje, aşağıdaki Python kütüphanelerini kullanmaktadır:

- numpy
- matplotlib
- sklearn
- scipy
## Gerekli kütüphaneleri yüklemek için:

pip install numpy matplotlib scikit-learn scipy
## Python Dosyasını Çalıştırma:

Projeyi çalıştırmak için aşağıdaki Python kodunu kullanabilirsiniz. Bu kod, verileri oluşturur, KMeans ve GMM algoritmalarını uygular ve sonuçları görselleştirir.

## Kod Açıklamaları
Veri Üretimi ve Hazırlığı
İlk olarak, make_blobs fonksiyonu ile 400 örnek içeren, dört merkez etrafında kümelenmiş yapay veri setleri üretilir. Veriler üzerinde rastgele bir gerilme (stretching) işlemi uygulanarak farklı bir dağılım elde edilir.

## KMeans Kümeleme
- KMeans Algoritması: KMeans algoritması, verileri 4 kümeye ayırır. Sonuçlar, her kümenin merkezini ve küme etiketlerini içerir.
- Görselleştirme: Kümelerin merkezleri ve küme etiketleri ile veri noktaları görselleştirilir. Küme merkezleri büyük kırmızı noktalarla gösterilir.
- Gaussian Mixture Model (GMM)
- GMM Algoritması: GaussianMixture modeli, verileri 4 Gauss dağılımı ile modellemeye çalışır.
- Elipsler ile Görselleştirme: Her Gauss bileşeni için elipsler çizilir. Elipsler, bileşenin veri üzerindeki etkisini ve kovaryansını temsil eder.
## Görselleştirme
Sonuçlar iki ayrı grafik üzerinde sunulur:

- Orijinal Veriler: Orijinal veri kümesi ve küme merkezleri.
- Gerilmiş Veriler: Gerilmiş veri kümesi ve algoritmaların performansı.
## Kodun Yapısı
Kod, aşağıdaki fonksiyonları içerir:

- plot_kmeans(kmeans, X): KMeans sonuçlarını çizer.
- plot_gmm(gmm, X): GMM sonuçlarını çizer.
- draw_ellipse(position, covariance, ax=None, **kwargs): Elipsleri çizer.
## Örnek Çıktılar
Kod çalıştırıldığında aşağıdaki gibi iki ana grafik elde edilir:

- KMeans Sonuçları: Küme merkezleri ve veri noktalarının renkli gösterimi.
- GMM Sonuçları: Gauss bileşenlerinin elipslerle temsil edildiği görselleştirme.
## Kullanım
Projeyi çalıştırmak için Python dosyasını aşağıdaki komut ile çalıştırabilirsiniz:


## Katkıda Bulunma
Herhangi bir katkıda bulunmak isterseniz, lütfen bir pull request gönderin veya buraya bir sorun açın.

## Lisans
Bu proje MIT Lisansı ile lisanslanmıştır.
