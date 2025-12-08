# MELY – Mücevher E-Ticaret Sitesi ve Yönetim Paneli

Bu proje kapsamında, hazır bir HTML/CSS şablonu kullanılarak **mücevher satışına yönelik bir web sitesi** ve bu siteyi yönetmek için bir **yönetim (admin) paneli** oluşturulmuştur. Başlangıçta fashion/e-ticaret için tasarlanmış tema, mücevher mağazası senaryosuna uyarlanmış; metinler, görseller, menüler ve kart yapıları projeye uygun şekilde düzenlenmiştir.

 **Canlı Demo:** https://MelikeSarii.github.io/Mucevher_Satis_Sitesi/

---

##  Projenin Amacı

- Hazır bir HTML/CSS & Bootstrap temasını alıp, **mücevher mağazası** konseptine uyarlamak  
- Müşterilerin ürünleri görebileceği **ön yüz (vitrin)** sayfasını tasarlamak  
- Site içeriklerinin ve bazı istatistiklerin yönetilebildiği bir **admin paneli** hazırlamak  
- CSS override, responsive tasarım ve tema özelleştirme konusunda pratik yapmak  

---

##  Özellikler

### Ön Yüz (Mücevher Sitesi)

- “Fashion store” teması mücevher temasına uyarlanmıştır.
- Ürün ve bölüm başlıkları mücevher odaklı hale getirilmiştir:
  - **Düğün Setleri**
  - **Özel Günler**
  - **Çok Satanlar** vb.
- Marka adı olarak **“Mely”** kullanılmıştır; sayfa başlıklarında ve metinlerde geçmektedir.
- Şablondaki İngilizce metinler Türkçeleştirilmiş, hedef kitleye uygun hale getirilmiştir.
- Görseller, mücevher konseptine uygun fotoğraflarla değiştirilmiştir.
- Kart görsellerinin boyutları ve oranları CSS ile düzenlenerek daha simetrik bir görünüm sağlanmıştır.
- Birimler ve Ürünler sayfaları için aynı şablon baz alınarak, başlıklar ve içerikler amaca göre uyarlanmıştır.
- Kıyafet temalı video, mücevher temalı bir video ile değiştirilmiştir.

### Yönetim Paneli (Admin)

- Admin paneli için kurumsal ve modern görünümlü bir yönetim teması kullanılmıştır.
- Sol menü başlıkları projeye uygun olacak şekilde Türkçeleştirilmiştir, örneğin:
  - **Mely Yönetim Paneli**
  - **Kontrol Paneli**
  - **Sayfalar / Sayfa Tasarımları**
  - **Hesap Hareketleri**
  - **Giriş & Güvenlik**
  - **Destek**
  - **Dokümantasyon**
- Mevcut kartlara ek olarak yeni kartlar eklenmiştir:
  - **Duyurular**
  - **Ürün Yönetimi**
  - **Görseller & Metinler** vb.
- Kartların başlıkları ve açıklamaları Türkçe ve anlamlı olacak şekilde güncellenmiştir.
- Kart yüksekliklerini eşitlemek için ek CSS sınıfları (örn. `card-equal`) kullanılmıştır.
- Tema rengi **mavi tonlarına** göre özelleştirilmiş, header ve bazı kart kenarlıkları bu renge göre ayarlanmıştır.
- Sol üstte yer alan tema adı (örn. “Sneat”, “ThemeSelection”) proje ismiyle uyumlu olacak şekilde değiştirilmiş ve yazı boyutu küçültülmüştür.

---

##  Kullanılan Teknolojiler

- **HTML5** – Sayfa yapısını oluşturmak için  
- **CSS3** – Tasarım, renkler, tipografi ve responsive yapı için  
- **Bootstrap 5** – Grid sistemi, kart yapıları ve hazır bileşenler için  
- **JavaScript (temel)** – Menü, küçük etkileşimler ve tema fonksiyonları için  
- **Git & GitHub** – Versiyon kontrolü ve **GitHub Pages** ile yayınlama için  

---

##  Proje Yapısı (Genel)

> Not: Aşağıdaki yapı örnek olup, kendi klasör yapına göre güncelleyebilirsin.

```text
proje-kök-dizini/
├─ index.html              # Ana vitrin sayfası (Mücevher sitesi)
├─ about.html              # Hakkımızda / Misyon-Vizyon
├─ contact.html            # İletişim sayfası
├─ products.html           # Ürünler / Koleksiyonlar
├─ units.html              # Birimler vb. (varsa)
├─ admin/                  # Yönetim paneli dosyaları
│  ├─ index.html           # Admin ana sayfa (dashboard)
│  ├─ pages/               # Admin alt sayfalar
│  └─ ...
├─ assets/
│  ├─ css/
│  │  ├─ style.css         # Tema ana stil dosyası
│  │  └─ custom.css        # Projeye özel override'lar
│  ├─ js/
│  ├─ img/
│  └─ video/
└─ README.md
 Kurulum ve Çalıştırma
Bu projeyi GitHub’dan clone veya download et:

bash
Kodu kopyala
git clone https://github.com/KULLANICI_ADIN/Mucevher_Satis_Sitesi.git
Proje klasörünü aç.

index.html dosyasını tarayıcı ile açarak ön yüzü görüntüleyebilirsin.

admin/index.html dosyasını açarak yönetim panelini görüntüleyebilirsin.

GitHub Pages üzerinden yayınlamak için:

Repo ayarlarından Pages sekmesine git.

“Deploy from a branch” → main branch + /root klasörünü seç.

Kaydet ve yayınlanan URL’yi kullan.

 Karşılaşılan Zorluklar & Çözümler
CSS override ve stil çakışmaları:

Hazır tema çok kapsamlı olduğu için bazı yeni CSS tanımları çalışmadı.

Tarayıcı geliştirici araçları ile doğru sınıflar tespit edildi, gerekli yerlerde !important kullanıldı.

Kart ve görsel boyutları:

Farklı oranlardaki görseller kart içinde hizalama problemi oluşturdu.

object-fit, sabit yükseklik gibi özelliklerle daha simetrik bir görünüm sağlandı.

Metinlerin İngilizce olması:

Vitrin sayfası ve admin panelindeki anlamsız görünen İngilizce terimler,
mücevher mağazası senaryosuna uygun Türkçe karşılıklarla değiştirildi.

 Gelecek Geliştirmeler
Projeye ileride aşağıdaki özellikler eklenebilir:

Gerçek bir veri tabanı entegrasyonu

Kullanıcı kayıt/giriş sistemi

Admin panelinden:

Ürün ekleme / silme / güncelleme

Sipariş takibi ekranları

Basit bir sepet ve ödeme simülasyonu

Mobil cihazlar için daha gelişmiş responsive iyileştirmeler

 Geliştirici
Melike Sarı – 231307102

Bu proje, hazır HTML/CSS temalarının gerçek bir senaryoya (mücevher e-ticareti) göre nasıl özelleştirilebileceğini göstermek amacıyla hazırlanmıştır.

Kodu kopyala

Kaynaklar

1/2







Şunu dedin:
 Kurulum ve Çalıştırma

burdan itibaren olan kısmı da koyayaım mı sadece üstteki kısmı mı koayayım


ChatGPT:
README dosyası için sadece üstteki kısmı koyman yeterli — yani benim sana verdiğim tüm içerik zaten tam bir README.

Ekstra bir şey eklemene gerek yok.
"Buradan itibaren" dediğin kısım ( Kurulum ve Çalıştırma, Zorluklar, Geliştirmeler, vb.) README’nin doğal parçasıdır, o yüzden tamamını aynen kopyalayıp README.md içine yapıştırmalısın.

Yani net cevap:
 Tüm verdiğim metni olduğu gibi README.md dosyana ekle.
 Sadece üst tarafı ekleme — aşağıdaki bölümler de README’nin önemli parçaları.

İstersen sana temizlenmiş, doğrudan GitHub’a yapıştırmalık halini tekrar tek parça verebilirim.







Şunu dedin:
olur


ChatGPT:
Tamam! Aşağıdaki metni OLDUĞU GİBİ kopyalayıp GitHub’daki README.md dosyana yapıştırabilirsin.
Hiçbir şey silme, değiştirmene gerek yok. Bu hazır ve profesyonel bir README’dir.

markdown
Kodu kopyala
# MELY – Mücevher E-Ticaret Sitesi ve Yönetim Paneli

Bu proje kapsamında, hazır bir HTML/CSS şablonu kullanılarak **mücevher satışına yönelik bir web sitesi** ve bu siteyi yönetmek için bir **yönetim (admin) paneli** oluşturulmuştur. Başlangıçta fashion/e-ticaret için tasarlanmış tema, mücevher mağazası senaryosuna uyarlanmış; metinler, görseller, menüler ve kart yapıları projeye uygun şekilde düzenlenmiştir.

 **Canlı Demo:** https://MelikeSarii.github.io/Mucevher_Satis_Sitesi/

---

##  Projenin Amacı

- Hazır bir HTML/CSS & Bootstrap temasını alıp, **mücevher mağazası** konseptine uyarlamak  
- Müşterilerin ürünleri görebileceği **ön yüz (vitrin)** sayfasını tasarlamak  
- Site içeriklerinin ve bazı istatistiklerin yönetilebildiği bir **admin paneli** hazırlamak  
- CSS override, responsive tasarım ve tema özelleştirme konusunda pratik yapmak  

---

##  Özellikler

### Ön Yüz (Mücevher Sitesi)

- “Fashion store” teması mücevher temasına uyarlanmıştır.
- Ürün ve bölüm başlıkları mücevher odaklı hale getirilmiştir:
  - **Düğün Setleri**
  - **Özel Günler**
  - **Çok Satanlar** vb.
- Marka adı olarak **“Mely”** kullanılmıştır; sayfa başlıklarında ve metinlerde geçmektedir.
- Şablondaki İngilizce metinler Türkçeleştirilmiş, hedef kitleye uygun hale getirilmiştir.
- Görseller, mücevher konseptine uygun fotoğraflarla değiştirilmiştir.
- Kart görsellerinin boyutları ve oranları CSS ile düzenlenerek daha simetrik bir görünüm sağlanmıştır.
- Birimler ve Ürünler sayfaları için aynı şablon baz alınarak, başlıklar ve içerikler amaca göre uyarlanmıştır.
- Kıyafet temalı video, mücevher temalı bir video ile değiştirilmiştir.

### Yönetim Paneli (Admin)

- Admin paneli için kurumsal ve modern görünümlü bir yönetim teması kullanılmıştır.
- Sol menü başlıkları projeye uygun olacak şekilde Türkçeleştirilmiştir, örneğin:
  - **Mely Yönetim Paneli**
  - **Kontrol Paneli**
  - **Sayfalar / Sayfa Tasarımları**
  - **Hesap Hareketleri**
  - **Giriş & Güvenlik**
  - **Destek**
  - **Dokümantasyon**
- Mevcut kartlara ek olarak yeni kartlar eklenmiştir:
  - **Duyurular**
  - **Ürün Yönetimi**
  - **Görseller & Metinler** vb.
- Kartların başlıkları ve açıklamaları Türkçe ve anlamlı olacak şekilde güncellenmiştir.
- Kart yüksekliklerini eşitlemek için ek CSS sınıfları (örn. `card-equal`) kullanılmıştır.
- Tema rengi **mavi tonlarına** göre özelleştirilmiş, header ve bazı kart kenarlıkları bu renge göre ayarlanmıştır.
- Sol üstte yer alan tema adı (örn. “Sneat”, “ThemeSelection”) proje ismiyle uyumlu olacak şekilde değiştirilmiş ve yazı boyutu küçültülmüştür.

---

##  Kullanılan Teknolojiler

- **HTML5** – Sayfa yapısını oluşturmak için  
- **CSS3** – Tasarım, renkler, tipografi ve responsive yapı için  
- **Bootstrap 5** – Grid sistemi, kart yapıları ve hazır bileşenler için  
- **JavaScript (temel)** – Menü, küçük etkileşimler ve tema fonksiyonları için  
- **Git & GitHub** – Versiyon kontrolü ve **GitHub Pages** ile yayınlama için  

---

##  Proje Yapısı (Genel)

```text
proje-kök-dizini/
├─ index.html              # Ana vitrin sayfası (Mücevher sitesi)
├─ about.html              # Hakkımızda / Misyon-Vizyon
├─ contact.html            # İletişim sayfası
├─ products.html           # Ürünler / Koleksiyonlar
├─ units.html              # Birimler vb. (varsa)
├─ admin/                  # Yönetim paneli dosyaları
│  ├─ index.html           # Admin ana sayfa (dashboard)
│  ├─ pages/               # Admin alt sayfalar
│  └─ ...
├─ assets/
│  ├─ css/
│  │  ├─ style.css         # Tema ana stil dosyası
│  │  └─ custom.css        # Projeye özel override'lar
│  ├─ js/
│  ├─ img/
│  └─ video/
└─ README.md
 Kurulum ve Çalıştırma
Bu projeyi GitHub’dan clone veya download et:

bash
Kodu kopyala
git clone https://github.com/KULLANICI_ADIN/Mucevher_Satis_Sitesi.git
Proje klasörünü aç.

index.html dosyasını tarayıcı ile açarak ön yüzü görüntüleyebilirsin.

admin/index.html dosyasını açarak yönetim panelini görüntüleyebilirsin.

GitHub Pages üzerinden yayınlamak için:

Repo ayarlarından Pages sekmesine git.

“Deploy from a branch” → main branch + /root klasörünü seç.

Kaydet ve yayınlanan URL’yi kullan.

 Karşılaşılan Zorluklar & Çözümler
CSS override ve stil çakışmaları:

Hazır tema çok kapsamlı olduğu için bazı yeni CSS tanımları çalışmadı.

Tarayıcı geliştirici araçları ile doğru sınıflar tespit edildi, gerekli yerlerde !important kullanıldı.

Kart ve görsel boyutları:

Farklı oranlardaki görseller kart içinde hizalama problemi oluşturdu.

object-fit, sabit yükseklik gibi özelliklerle daha simetrik bir görünüm sağlandı.

Metinlerin İngilizce olması:

Vitrin sayfası ve admin panelindeki anlamsız görünen İngilizce terimler,
mücevher mağazası senaryosuna uygun Türkçe karşılıklarla değiştirildi.

 Gelecek Geliştirmeler
Veri tabanı entegrasyonu

Ürün ekleme / silme / güncelleme

Sipariş takibi ekranları

Kullanıcı kayıt/giriş sistemi

Sepet & ödeme simülasyonu

Mobil görünüm için gelişmiş responsive iyileştirmeler

 Geliştirici
Melike Sarı – 231307102

Bu proje, hazır HTML/CSS temalarının gerçek bir senaryoya (mücevher e-ticareti) göre nasıl özelleştirilebileceğini göstermek amacıyla hazırlanmıştır.
