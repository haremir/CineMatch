# IMDB Puanlarına Dayalı Film Tavsiye Sistemi

## Proje Özeti

Bu proje, IMDB film puanlarına dayalı bir film tavsiye sistemi geliştirmeyi amaçlamaktadır. Kullanıcıların puanlarına ve film benzerliklerine dayanarak kişiselleştirilmiş film önerileri sunan bir sistem oluşturulmuştur. Proje, veri ön işleme, korelasyon analizi ve benzerlik hesaplamalarını içerir.

## İçindekiler

- [IMDB Puanlarına Dayalı Film Tavsiye Sistemi](#imdb-puanlarına-dayalı-film-tavsiye-sistemi)
  - [Proje Özeti](#proje-özeti)
  - [İçindekiler](#i̇çindekiler)
  - [Veri Setleri](#veri-setleri)
  - [Proje Adımları](#proje-adımları)
  - [Görselleştirmeler](#görselleştirmeler)
  - [Kurulum ve Kullanım](#kurulum-ve-kullanım)
  - [Yazarlar](#yazarlar)

## Veri Setleri

Projede iki ana veri seti kullanılmaktadır:

1. **Kullanıcı Derecelendirmeleri:**
   - `user_id`: Kullanıcı kimliği
   - `item_id`: Film kimliği
   - `rating`: Kullanıcı tarafından verilen puan
   - `timestamp`: Derecelendirmenin yapıldığı zaman

| user_id | item_id | rating | timestamp |
|---------|---------|--------|-----------|
| 0       | 50      | 5      | 881250949 |
| 0       | 172     | 5      | 881250949 |
| 0       | 133     | 1      | 881250949 |
| 196     | 242     | 3      | 881250949 |
| 186     | 302     | 3      | 891717742 |



1. **Film Bilgileri:**
- `item_id`: Film kimliği
- `title`: Filmlerin isimleri

| item_id | title                        |
|---------|------------------------------|
| 1       | Toy Story (1995)             |
| 2       | GoldenEye (1995)             |
| 3       | Four Rooms (1995)            |
| 4       | Get Shorty (1995)            |
| 5       | Copycat (1995)               |


## Proje Adımları

1. **Veri Ön İşleme:**
- Verilerin birleştirilmesi ve temizlenmesi
- Zaman damgalarının dönüştürülmesi

2. **Korelasyon ve Benzerlik Hesaplama:**
- Film filmleri arasındaki korelasyon hesaplamaları
- Cosine benzerlik ölçütü ile film benzerliklerinin hesaplanması

3. **Görselleştirme:**
- Korelasyon ve oy sayıları grafiklerinin oluşturulması

4. **Öneri Sistemi:**
- Kullanıcının seçtiği filme göre öneri yapılması
- En yüksek benzerlik skorlarına sahip 10 film önerisi

## Görselleştirmeler

- **Korelasyon Grafiği:**
![Korelasyon Grafiği](link-to-your-graph1.png)
*Görsel 1: Film Korelasyon Grafiği*

- **Film Oy Sayısı Grafiği:**
![Film Oy Sayısı Grafiği](link-to-your-graph2.png)
*Görsel 2: Film Oy Sayısı Grafiği*

## Kurulum ve Kullanım

1. **Gereksinimler:**
- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Scikit-learn

2. **Kurulum:**
pip install pandas numpy matplotlib scikit-learn


3. **Projeyi Çalıştırma:**
- Repo'yu klonlayın:
  ```
  git clone https://github.com/harunemirhan/film-tavsiye-sistemi.git
  ```
- Ana dosyayı çalıştırın:
  ```
  python main.py
  ```

## Yazarlar

- Harun Emirhan - [LinkedIn Profilim](https://www.linkedin.com/in/harun-emirhan-bostanci-24144726b/)
