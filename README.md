# 🎬 Film ve Dizi Takip Uygulaması (Scraper Destekli)

Bu uygulama, kullanıcıların izledikleri veya izlemeyi planladıkları film ve dizileri modern bir arayüzle kayıt altına almalarını sağlayan profesyonel bir Python masaüstü uygulamasıdır. **sinemalar.com** entegrasyonu sayesinde film bilgilerini manuel girmek yerine otomatik olarak çekebilir.

## ✨ Öne Çıkan Özellikler

- **🚀 Akıllı Veri Çekme (Web Scraping):** Film ekleme ekranında bir **sinemalar.com** linki paylaştığınızda; film adı, çıkış yılı, özet bilgisi ve afiş resmi otomatik olarak internetten çekilir.
- **🎨 Modern ve Dinamik Arayüz:** CustomTkinter kütüphanesi ile geliştirilmiş, kullanıcı dostu ve şık tasarım.
- **⭐ Kişisel Puanlama:** İzlediğiniz içeriklere 5 yıldız üzerinden puan verebilme ve bu puanları dilediğiniz zaman güncelleyebilme.
- **🖼️ Görsel Kütüphane:** Her film/dizi için poster desteği ile görsel bir arşiv oluşturma.
- **📂 Düzenleme ve Silme:** Kayıtlı içeriklerin tüm bilgilerini sonradan değiştirebilme veya tamamen kaldırabilme.
- **🔒 Yerel Veri Yönetimi:** Verileriniz `database.json` dosyasında yerel olarak saklanır, veritabanı kurulumu gerektirmez.

## 🛠️ Kullanılan Teknolojiler

- **Dil:** Python 3.11+
- **GUI:** [CustomTkinter](https://github.com/TomSchimansky/CustomTkinter) (Modern Tkinter Arayüzü)
- **Scraping:** `BeautifulSoup4` & `Requests` (sinemalar.com verilerini işlemek için)
- **Görüntü İşleme:** `Pillow` (PIL) (Afişlerin boyutlandırılması ve gösterimi için)
- **Depolama:** JSON Formatı

## 📁 Proje Yapısı

```text
├── database/           # Veri saklama (JSON) ve Poster klasörleri
├── models/             # Film nesne modeli (filmModel.py)
├── services/           # Arka plan mantığı
│   ├── database.py     # JSON okuma/yazma işlemleri
│   └── request.py      # Sinemalar.com scraping motoru
├── views/              # UI Bileşenleri (Sayfalar, Kartlar, Formlar)
├── main.py             # Uygulama başlangıç dosyası
└── requirements.txt    # Bağımlılıklar
```

## 🚀 Kurulum ve Çalıştırma

1. **Projeyi indirin:**
   ```bash
   git clone [https://github.com/muhammedkizildag/film-dizi-takip-uygulamasi.git](https://github.com/muhammedkizildag/film-dizi-takip-uygulamasi.git)
   cd film-dizi-takip-uygulamasi
   ```

2. **Bağımlılıkları yükleyin:**
   ```bash
   pip install customtkinter pillow beautifulsoup4 requests
   ```

3. **Çalıştırın:**
   ```bash
   python main.py
   ```

## 📖 Nasıl Kullanılır?

1. **Otomatik Ekleme:** Sol menüden "Film Ekle"ye tıklayın. Açılan formdaki "URL" alanına bir **sinemalar.com** film linki yapıştırın ve "Verileri Çek" butonuna basın. Bilgiler saniyeler içinde dolacaktır.
2. **Manuel Kayıt:** Eğer internet verisi kullanmak istemiyorsanız, tüm alanları kendiniz doldurup yerel bir resim seçebilirsiniz.
3. **Arşiv Yönetimi:** Ana sayfada kartlar üzerinde bulunan simgeleri kullanarak puan verebilir, bilgileri düzenleyebilir veya filmi silebilirsiniz.


https://github.com/user-attachments/assets/e4ecdc6c-2e87-4313-961c-07753034bb45


---
Geliştiren: **[Muhammed Kızıldağ]**
