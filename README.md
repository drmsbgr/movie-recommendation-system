# 🎬 Movie Recommendation System (Film Öneri Sistemi)

![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-orange)
![Library](https://img.shields.io/badge/Library-Scikit--Learn-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 📌 Proje Konusu
Bu proje, **Veri Madenciliği ve Bilgi Keşfi** dersi kapsamında geliştirilmiş bir içerik bazlı (content-based) film öneri sistemidir. Sistem, kullanıcıların ilgilendikleri bir filmi girdi olarak alır ve doğal dil işleme (NLP) tekniklerini kullanarak içerik/tür açısından en benzer filmleri önerir.

Temel amaç; büyük veri setleri üzerinde metin madenciliği tekniklerini uygulayarak, **soğuk başlangıç (cold-start)** problemini aşan ve kullanıcı geçmişinden bağımsız öneriler sunabilen bir motor geliştirmektir.

## 👨‍💻 Geliştirici
* **Adı Soyadı:** Buğra DURMUŞ
* **Öğrenci No:** 231118013
* **Bölüm/Ders:** Yazılım Mühendisliği / Veri Madenciliği ve Bilgi Keşfi

## ⚙️ Kullanılan Yöntemler ve Teknolojiler

Projede **İçerik Bazlı Filtreleme (Content-Based Filtering)** yaklaşımı benimsenmiştir. Kullanılan temel algoritmalar ve kütüphaneler şunlardır:

### 1. Teknolojiler
* **Python:** Projenin ana programlama dili.
* **Pandas:** Veri manipülasyonu ve temizleme işlemleri (Dataframe yönetimi).
* **Scikit-learn:** Makine öğrenmesi algoritmaları ve vektörleştirme işlemleri.
* **Google Colab:** Geliştirme ortamı.

### 2. Algoritmalar ve Teknikler
* **TF-IDF (Term Frequency-Inverse Document Frequency):** Filmlerin tür (genre) bilgilerini metin formatından sayısal vektörlere dönüştürmek için kullanılmıştır. Bu yöntem, sık geçen kelimelerin ağırlığını azaltıp ayırt edici özelliklerin ağırlığını artırır.
* **Cosine Similarity (Kosinüs Benzerliği):** Filmler arasındaki benzerliği ölçmek için kullanılmıştır. Vektör uzayında iki film vektörü arasındaki açının kosinüsünü hesaplayarak 0 ile 1 arasında bir benzerlik skoru üretir.

## 📊 Veri Seti Kaynağı

Projede GroupLens Research tarafından sağlanan **MovieLens** veri seti kullanılmıştır.

* **Veri Seti Adı:** MovieLens Latest Small Dataset
* **İçerik:** 100.000 derecelendirme, 3.600 etiket, 9.000+ film.
* **Kaynak Linki:** [MovieLens Datasets](https://grouplens.org/datasets/movielens/latest/)
* **Citation:** *F. Maxwell Harper and Joseph A. Konstan. 2015. The MovieLens Datasets: History and Context. ACM Transactions on Interactive Intelligent Systems (TiiS) 5, 4: 19:1–19:19.*

## 🚀 Kurulum ve Çalıştırma

Proje Google Colab üzerinde çalıştırılmak üzere tasarlanmıştır, ancak yerel ortamda çalıştırmak isterseniz:

1.  Bu repoyu klonlayın:
    ```bash
    git clone https://github.com/drmsbgr/movie-recommendation-system.git
    ```
2.  Gerekli kütüphaneleri yükleyin:
    ```bash
    pip install pandas numpy scikit-learn
    ```
3.  `main.py` veya `.ipynb` dosyasını çalıştırın.

## 📈 Örnek Çıktı

Sisteme **"Toy Story (1995)"** filmi verildiğinde üretilen örnek öneriler:

1.  Antz (1998)
2.  Toy Story 2 (1999)
3.  The Incredibles (2004)
4.  Monsters, Inc. (2001)
...

---
*Bu proje Veri Madenciliği ve Bilgi Keşfi dersi kapsamında hazırlanmıştır.*
