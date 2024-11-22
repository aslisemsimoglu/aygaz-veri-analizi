# **Los Angeles Suç Verisi Analizi** 🔍

### **Proje Hakkında**

Bu proje, Los Angeles'taki suç verilerini analiz ederek suç türlerinin zaman ve mekânsal dağılımlarını anlamayı, veri analitiği ve görselleştirme becerilerini geliştirmeyi amaçlamaktadır. Aygaz Veri Analizi Proje Kampı kapsamında yürütülen bu çalışma, suç verileriyle derinlemesine içgörüler elde etmeye yönelik kapsamlı bir veri analizi içermektedir.

----------

## **Proje Ekibi**

-   **Aslı Şemşimoğlu**:  
    Afyon Kocatepe Üniversitesi Bilgisayar Mühendisliği 4. sınıf öğrencisiyim. Özellikle **doğal dil işleme (NLP)** ve **makine öğrenimi** üzerine projeler geliştiriyorum. Kaggle'da aktif bir kullanıcı olarak veri analitiği projelerine katkı sağlamaktan büyük keyif alıyorum. 
-   **Berke Çelebi**:  
    Fenerbahçe Üniversitesi Yönetim Bilişim Sistemleri 3. sınıf öğrencisiyim. Özellikle **makine öğrenimi** ve **veri analitiği** konularında projeler geliştiriyorum. Aldığım eğitimler ve üzerinde çalıştığım projelerle bu alandaki bilgimi derinleştirmekten büyük keyif alıyorum. 

----------

## **Projenin Amacı**

1.  **Suç Verilerini İncelemek**:  
    Suçların zaman, mekân ve türlerine göre dağılımlarını analiz ederek suç oranları üzerine içgörüler sağlamak.
2.  **Veriyi Görselleştirmek**:  
    Etkileşimli haritalar ve grafikler ile veriyi kullanıcı dostu bir şekilde görselleştirmek.
3.  **İstatistiksel Bağlantılar Kurmak**:  
    Suç türleri ile yakalanma oranları arasındaki ilişkileri keşfetmek.

----------

## **Veri Seti Bilgileri**

-   **Los Angeles Suç Verisi (2020 - Günümüz):**
    -   **Kapsam**: 944,235 kayıt ve 28 sütun.
    -   **Özellikler**: Suç türü, mekânsal koordinatlar (LAT, LON), olay zamanı, yakalama durumu vb.
    -   **Eksiklikler**: Bazı sütunlarda eksik veri (örneğin, `Weapon Desc`, `Vict Sex`).
-   **Chicago Suç Verisi** (isteğe bağlı analiz için).

----------

## **Proje Akışı**

### 1. **Veri Ön İşleme**

-   Eksik verilerin analiz edilmesi ve doldurulması.
-   Tarih sütunlarının datetime formatına dönüştürülmesi.
-   Kategorik ve sayısal sütunların otomatik tespiti.

### 2. **Keşifsel Veri Analizi (EDA)**

-   Suçların mekânsal dağılımı: Folium ile ısı haritaları.
-   Zaman serileri analizi: Yıllara, aylara ve haftanın günlerine göre suç oranlarının incelenmesi.
-   Suç türleri ve frekans dağılımları: Çubuk ve pasta grafikleri.

### 3. **Feature Engineering**

-   Tarih bilgilerini zenginleştirme: Yıl, ay, gün sütunları ekleme.
-   Olay başına suç kodu sayısının hesaplanması.

### 4. **Veri Görselleştirme**

-   Folium ile suç haritaları.
-   Seaborn ve Matplotlib ile interaktif grafikler.

----------

## **Görselleştirme Çıktıları**

### 🔍 **Harita Analizleri**

-   **Genel Suç Yoğunluğu**: Los Angeles’ın merkezinde yoğunlaşan suçları gösteren ısı haritaları.
-   **Hırsızlık Yoğunluğu**: Yalnızca hırsızlık verilerini filtreleyerek suç noktalarının görselleştirilmesi.

### 📊 **Grafikler**

-   **En Yaygın Suç Türleri**: İlk 30 suç türünü ve oranlarını gösteren çubuk grafiği.
-   **Haftanın Günlerine Göre Suç Dağılımı**: Suçların hafta içi ve hafta sonu dağılımlarını analiz eden yatay grafikler.
-   **Aylık Suç Dağılımı**: Suçların yıl boyunca aylara göre nasıl değiştiğini analiz eden grafik.

----------

## **Kullanılan Teknolojiler ve Kütüphaneler**

-   **Python**: Veri analitiği ve görselleştirme için temel programlama dili.
-   **Pandas & NumPy**: Veri işleme ve analiz.
-   **Seaborn & Matplotlib**: Görselleştirme araçları.
-   **Folium**: Harita tabanlı suç yoğunluğu analizleri.

----------

## **Sonuçlar ve Öneriler**

-   **Yıllık Suç Trendleri**: 2020’den itibaren suç oranlarında düşüş gözlemlenmiştir.
-   **Suç Yoğunluğu Bölgeleri**: Şehir merkezi ve belirli mahalleler suç oranlarının en yoğun olduğu alanlardır.
-   **Eksik Veri Yönetimi**: Eksik veriler için uygun doldurma stratejileri uygulanmıştır.

Bu analiz, Los Angeles suç verilerinin farklı perspektiflerden anlaşılmasını sağlamış ve veri analitiği süreçlerinde pratik deneyim kazandırmıştır.

----------

## **Kurulum**

Projeyi yerel bir ortamda çalıştırmak için:

1.  Gerekli Python kütüphanelerini yükleyin:
    
    bash
    
    Kodu kopyala
    
    `pip install pandas numpy seaborn matplotlib folium` 
    
2.  Veri setlerini proje dosyasıyla aynı dizine yerleştirin.
3.  Notebook’u çalıştırarak adım adım analizi takip edin.

----------

## **Proje Özeti**

Los Angeles Suç Verisi Analizi projesi, verinin gücünü kullanarak şehirdeki suç oranlarını daha iyi anlamak için güçlü bir araçtır. Folium ile görselleştirme ve Seaborn ile grafik analizleri sayesinde, suç verilerinin kullanıcı dostu bir şekilde sunulması sağlanmıştır.

🎉 **Teşekkürler!**
