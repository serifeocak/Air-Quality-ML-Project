# 🌍 Makine Öğrenmesi Yöntemleri ile Hava Kalitesi Analizi  

## 📌 Proje Tanıtımı  
Bu proje, **SAP** ve **Teknolojide Kadın Derneği** iş birliğiyle yürütülen  
**“Güçlü Kadınlarla Dijital Yarınlar – Python ile Yapay Zeka Eğitim Programı”** kapsamında hazırlanan bir bitirme projesidir.  

Projenin temel amacı, çeşitli çevresel parametreleri kullanarak **hava kalitesini sınıflandırmak ve tahmin etmek** için makine öğrenmesi algoritmalarının etkinliğini analiz etmektir.  

---

## 🎯 Hedef ve Veri Seti  

### 🎯 Hedef Değişken  
Hava kalitesi, **çok sınıflı sınıflandırma** problemine göre 4 ana sınıfa ayrılmıştır:  
- **Good (İyi)**  
- **Moderate (Orta)**  
- **Poor (Kötü)**  
- **Hazardous (Tehlikeli)**  

### 📊 Veri Kaynağı ve Özellikler  
- **Kaynak:** [Kaggle - Air Quality and Pollution Assessment](https://www.kaggle.com/)  
- **Özellikler:**  
  - Sıcaklık (Temperature)  
  - Nem (Humidity)  
  - Partikül Maddeler (PM2.5, PM10)  
  - Gaz Kirlilikleri (NO2, SO2, CO)  
  - Nüfus Yoğunluğu (Population_Density)  
  - Sanayi Alanlarına Yakınlık (Proximity_to_Industrial_Areas)  

---

## 🛠️ Metodoloji  

Proje, standart bir veri bilimi iş akışını takip etmektedir:  

### 1️⃣ Veri Ön İşleme ve Analiz  
- **Keşifsel Veri Analizi (EDA):** Veri yapısı, korelasyonlar ve sınıf dağılımı incelendi.  
- **Eksik Değer Yönetimi:** Veri setinde eksik değer bulunmadı.  
- **Aykırı Değer Analizi:** Kutu grafikleriyle aykırı değerler analiz edildi.  
- **Kodlama & Ölçeklendirme:**  
  - Hedef değişken (*Air Quality*) → Label Encoding  
  - Bağımsız değişkenler → StandardScaler  

### 2️⃣ Boyut İndirgeme  
Yüksek boyutlu veriyi görselleştirmek ve model performansına etkisini test etmek için:  
- **PCA (Principal Component Analysis)**  
- **LDA (Linear Discriminant Analysis)**  
- **t-SNE (t-distributed Stochastic Neighbor Embedding)**  

### 3️⃣ Makine Öğrenmesi Modelleri  
Karşılaştırılan sınıflandırma algoritmaları:  
- Lojistik Regresyon  
- K-En Yakın Komşu (KNN)  
- Karar Ağacı (Decision Tree)  
- Rastgele Orman (Random Forest)  
- Destek Vektör Makineleri (SVM)  

### 4️⃣ Gelişmiş Teknikler  
- **Düzenlileştirme (Regularization):**  
  - Lojistik Regresyon → L1 & L2  
  - SVM → C parametresi  
- **Kümeleme Analizi (Unsupervised):**  
  - K-Means  
  - DBSCAN  

---

## 🏆 Temel Çıkarımlar  
- **Rastgele Orman** ve **SVM**, sınıflandırma görevinde en yüksek başarıyı göstermiştir.  
- Düzenlileştirme teknikleri, **genelleştirme yeteneğini artırmıştır.**  
- **LDA** ile boyut indirgeme, verilerin ayrıştırılmasında ve görselleştirilmesinde etkili olmuştur.  

---

## 🚀 Kullanılan Teknolojiler  
Projede kullanılan başlıca teknolojiler ve kütüphaneler şunlardır:  

- **Programlama Dili:** Python  
- **Veri Analizi:** NumPy, Pandas  
- **Makine Öğrenmesi:** Scikit-learn  
- **Görselleştirme:** Matplotlib, Seaborn  
- **Boyut İndirgeme:** PCA, LDA, t-SNE  
- **Kümeleme:** K-Means, DBSCAN  

---


