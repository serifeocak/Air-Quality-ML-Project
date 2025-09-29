Makine Öğrenmesi Yöntemleri ile Hava Kalitesi Analizi
🌟 Proje Tanıtımı
Bu proje, 

SAP ve Teknolojide Kadın Derneği iş birliğiyle yürütülen “Güçlü Kadınlarla Dijital Yarınlar” Python ile Yapay Zeka Eğitim Programı kapsamında hazırlanan bir bitirme projesidir.

Projenin temel amacı, çeşitli çevresel parametre verilerini kullanarak hava kalitesini doğru bir şekilde 

sınıflandırmak ve tahmin etmek için makine öğrenmesi (ML) algoritmalarının etkinliğini analiz etmektir.

🎯 Hedef ve Veri Seti
Hedef Değişken
Hava kalitesini dört ana sınıfa (Çoklu Sınıflandırma) ayırmaktır:

Good (İyi)

Moderate (Orta)

Poor (Kötü)

Hazardous (Tehlikeli)

Veri Kaynağı ve Özellikler

Kaynak: Kaggle - Air Quality and Pollution Assessment.


Temel Özellikler: Sıcaklık (Temperature), Nem (Humidity), Partikül Maddeler (PM2.5, PM10), Gaz Kirlilikleri (NO2, SO2, CO), Nüfus Yoğunluğu (Population_Density) ve Sanayi Alanlarına Yakınlık (Proximity_to_Industrial_Areas) gibi çevresel ve demografik veriler kullanılmıştır.

🛠️ Metodoloji ve Uygulanan Teknikler
Proje, standart bir veri bilimi iş akışını takip etmektedir:

1. Veri Ön İşleme ve Analiz

Keşifsel Veri Analizi (EDA): Veri setinin yapısı, korelasyonları ve sınıf dağılımı incelenmiştir.




Eksik Değer Yönetimi: Veri setinde eksik değere rastlanmamıştır.



Aykırı Değer Analizi: Model performansını korumak için kutu grafikleriyle aykırı değerler analiz edilmiştir.



Kodlama ve Ölçeklendirme: Kategorik hedef değişken (Air Quality) Label Encoding ile , bağımsız değişkenler ise 

StandardScaler ile standardizasyon yapılarak ölçeklendirilmiştir.

2. Boyut İndirgeme
Yüksek boyutlu veriyi görselleştirmek ve model performansına etkisini test etmek için kullanılmıştır.



PCA (Temel Bileşen Analizi) 


LDA (Lineer Diskriminant Analizi) 


t-SNE (t-Dağılımlı Stokastik Komşu Gömme) 

3. Makine Öğrenmesi Modelleri
Hava kalitesi sınıflamasını yapmak için çeşitli sınıflandırma algoritmaları karşılaştırılmıştır:

Lojistik Regresyon

K-En Yakın Komşu (KNN)

Karar Ağacı (Decision Tree)

Rastgele Orman (Random Forest)

Destek Vektör Makineleri (SVM)

4. Gelişmiş Teknikler

Düzenlileştirme (Regularization): Aşırı öğrenmeyi (overfitting) önlemek için Lojistik Regresyon için L1 ve L2, SVM için C parametresi gibi teknikler denenmiştir.



Kümeleme Analizi: Veri içindeki doğal grupları ve gizli desenleri denetimsiz bir şekilde keşfetmek için K-Means ve DBSCAN algoritmaları kullanılmıştır.

🏆 Temel Çıkarımlar
Sınıflandırma görevinde en başarılı sonuçları 

Rastgele Orman ve SVM modelleri vermiştir.


Düzenlileştirme teknikleri, modellerin genelleştirme yeteneğini önemli ölçüde artırmıştır.


Boyut indirgeme (özellikle LDA), veriyi daha iyi ayrıştırmaya ve görselleştirmeye olanak tanımıştır.