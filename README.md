# veri_analizi
Bu kod, bir otel rezervasyon veri seti üzerinde eksik veri işleme, temel veri analizi, istatistiksel özetleme ve bazı özellik mühendisliği adımlarını içeriyor. 
Veri Yükleme ve Hazırlık:

pandas kullanarak veri seti yükleniyor ve ilk gözlemler inceleniyor.
Veri tipleri ve istatistiksel özetler alınıyor.
Eksik Veri Oluşturma ve İşleme:

add_random_missing_values fonksiyonu kullanılarak veri setine rastgele eksik değerler (NaN) ekleniyor.
Eksik veriler inceleniyor ve görselleştiriliyor.
Eksik veriler iki şekilde işleniyor:
Eksik veriye sahip satırlar kaldırılıyor (dropna()).
Eksik veriler, sayısal sütunlar için medyan ile dolduruluyor.
Korelasyon Analizi:

Sayısal sütunlar seçilerek, bunlar arasındaki korelasyon matrisini hesaplanıyor ve görselleştiriliyor.
Korelasyonu yüksek olan sütunlar belirleniyor ve bu sütunlar çıkarılıyor.
Özellik Mühendisliği:

Rezervasyon bekleme süresini ve lider zamanı toplayarak total_wait_time adlı yeni bir özellik oluşturuluyor.
Model Önerisi
Bu tür otel rezervasyon verileriyle şu analizler yapılabilir:

Klasifikasyon Modeli:

Örneğin, müşterilerin iptal eğilimlerini tahmin etmek için bir klasifikasyon modeli (lojistik regresyon, karar ağaçları, Random Forest veya Gradient Boosting gibi) kullanılabilir.
Hedef değişken olarak is_canceled (eğer varsa) gibi bir sütun kullanılabilir.
Regresyon Modeli:

Eğer müşteri bekleme süresini veya rezervasyon süresini tahmin etmek istiyorsanız, doğrusal regresyon veya Random Forest Regressor gibi algoritmalar kullanılabilir.
Hedef değişken, total_wait_time veya lead_time olabilir.
Öneri:

Random Forest veya Gradient Boosting modelleri, özellikle kategorik ve sayısal verilerle iyi performans gösterir.
Veriyi modellemeye uygun hale getirdikten sonra train_test_split ile eğitim ve test setlerine ayırabilir ve model performansını değerlendirebilir.


https://www.kaggle.com/code/nurayerdogan/veri-analizi
