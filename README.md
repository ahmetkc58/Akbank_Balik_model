Bu proje, Akbank Deep Learning Bootcamp kapsamında geliştirilmiş olup, çeşitli balık türlerini içeren bir görüntü veri seti kullanarak balık sınıflandırması yapmayı amaçlamaktadır. Yapay sinir ağı (ANN) modeli kullanılarak yüksek doğrulukta bir sınıflandırıcı modeli geliştirilmiştir.

🐟 Kaggle üzerindeki projeme buradan ulaşabilirsiniz.

Proje Özeti
Veri Hazırlama ve Keşifsel Veri Analizi (EDA)

Veri Setinin Yüklenmesi: Projenin temelini, Kaggle'dan alınan balık görüntü veri seti oluşturmaktadır. Veri setindeki balık türleri, her biri farklı klasörlerde yer almakta.
Veri Seti Organizasyonu: Balık türlerine ait görüntü dosyalarının yolları ve sınıf etiketleri (balık türleri), Python kullanılarak düzenlenmiş ve Pandas DataFrame'e dönüştürülmüştür.
Veri Keşfi (EDA): Veri setindeki balık türlerinin sayısı ve her sınıfa ait görüntülerin dağılımı analiz edilmiştir. Veri dengesizliği durumunda, veri artırma (data augmentation) yöntemleri ile çözüm sağlanması planlanmıştır.
Veri Ön İşleme

Etiketleme: Balık türlerine göre görüntüler etiketlenmiş ve eğitim sırasında kullanılmak üzere düzenlenmiştir.
Veri Setinin Bölünmesi: Veri seti, eğitim ve test seti olarak ayrılmıştır. Eğitim seti modelin öğrenmesi için, test seti ise modelin doğruluğunu değerlendirmek için kullanılmıştır.
Veri Artırma (Augmentation): Eğitim verileri üzerinde dönüşüm işlemleri (döndürme, aynalama gibi) uygulanarak, modelin daha geniş bir veri çeşitliliğiyle eğitilmesi sağlanmıştır.
Model Geliştirme ve Eğitim

Yapay Sinir Ağı (ANN) Modeli: TensorFlow ve Keras kullanılarak, balık görüntülerini sınıflandırmak üzere bir yapay sinir ağı modeli geliştirilmiştir.
Model Mimarisi: Modeldeki katman sayısı, aktivasyon fonksiyonları (ReLU, Softmax vb.), optimizer (örneğin, Adam), ve kayıp fonksiyonu (categorical crossentropy) belirlenmiş ve eğitim optimize edilmiştir.
Eğitim Süreci: Model, eğitim verileri üzerinde eğitilmiş ve doğrulama seti kullanılarak performansı izlenmiştir. Eğitim sırasında doğruluk (accuracy) ve kayıp (loss) gibi metrikler takip edilmiştir.
Model Değerlendirme

Başarı Metrikleri: Modelin performansı şu metriklerle değerlendirilmiştir:
Accuracy (Doğruluk): Modelin genel başarı oranı.
Confusion Matrix (Karmaşıklık Matrisi): Her sınıf için doğru ve yanlış sınıflandırmalar.
Classification Report (Sınıflandırma Raporu): Precision, recall, F1-score gibi metrikler kullanılarak modelin başarısı ölçülmüştür.
Model Optimizasyonu: Eğitim sırasında overfitting’in önlenmesi amacıyla doğrulama seti kullanılmış ve gerekli durumlarda erken durdurma (early stopping) ve düzenleme (regularization) gibi yöntemler uygulanmıştır.
Sonuçlar ve Yorumlar
Bu proje ile geliştirilen yapay sinir ağı modeli, balık türlerini yüksek doğruluk oranıyla sınıflandırmayı başarmıştır. Veri artırma ve optimizasyon teknikleri ile model daha da güçlendirilmiş ve elde edilen sonuçlar başarıyla değerlendirilmiştir. Sonuç olarak, bu model balık türlerini otomatik olarak ayırt etmek için etkili bir çözüm sunmaktadır.

Kullanılan Teknolojiler
Python: Veri işleme, model geliştirme ve analiz süreçlerinde.
TensorFlow & Keras: Yapay sinir ağı modelinin oluşturulması ve eğitimi.
Pandas & NumPy: Veri manipülasyonu ve düzenleme işlemleri.
Matplotlib & Seaborn: Veri görselleştirme ve analiz.
Sklearn: Model değerlendirme metrikleri (confusion matrix, accuracy, classification report).
Bu proje, Melike Nur ÇOTAK ile birlikte gerçekleştirilmiştir.
