# Staj-Projeleri

# 🚀 Kurumsal Veri Yönetimi ve İletişim Sistemleri

Bu depo, kurum içi operasyonları dijitalleştirmek, veri akışını hızlandırmak ve bilgi yönetimini optimize etmek amacıyla geliştirilen iki farklı Front-End (SPA) web uygulamasını içermektedir. Projeler, herhangi bir dış veritabanı veya sunucu gereksinimi duymadan, doğrudan tarayıcı mimarisi üzerinde dinamik veri yönetimi yapabilmek üzere tasarlanmıştır.

## 📂 Projeler

### 1. ONKA Dahili Telefon Rehberi (`rehber.html`)
İnsan Kaynakları departmanı için geliştirilen, kurum içi personelin iletişim ve özlük verilerini barındıran dinamik sistemdir.
* Kullanıcıların isim, dahili hat, departman ve e-posta gibi verilerini hızlıca tablo formatında listeler.
* Akıllı kopyalama algoritması ile tablodaki verilere tıklandığında anında panoya (clipboard) kopyalama işlemi yapar.

### 2. Satın Alma E-Posta Kayıt Sistemi (`eposta.html`)
Kurumun dış paydaşlarla (Müşteri, Tedarikçi, İş Ortağı) olan iletişim ağını loglamak için kurgulanmıştır.
* Kayıtları kategorik (müşteri, tedarikçi vb.) olarak renkli etiketlerle (badge) sınıflandırır.
* İlgili firmalara ait iletişim geçmişinin merkezi bir noktadan yönetilmesini sağlar.

## ✨ Öne Çıkan Teknik Özellikler

* **Tarayıcı Tabanlı Veritabanı (LocalStorage):** Veriler sunucuya ihtiyaç duymadan cihazın yerel önbelleğinde `JSON` formatında şifrelenerek tutulur, sayfayı yenilemek veri kaybına yol açmaz.
* **Veri İçe/Dışa Aktarma (ETL):** Sistemdeki mevcut kayıtlar Microsoft Excel uyumlu `CSV` formatında toplu olarak indirilebilir. Aynı zamanda dışarıdan hazırlanmış `.csv` dosyaları sisteme tek tıkla entegre edilebilir (Import/Export).
* **Gelişmiş Arama ve Filtreleme:** Departman veya kategori bazlı filtreleme seçeneklerinin yanında, tüm veri metinleri üzerinde anlık (real-time) arama yapabilen dinamik bir arama motoru içerir.
* **Karanlık Mod (Dark Mode):** Kullanıcı deneyimini (UX) artırmak adına, işletim sisteminin renk tercihiyle entegre çalışan veya manuel tetiklenebilen aydınlık/karanlık mod desteği mevcuttur.
* **Hata Yönetimi (Undo/Toast):** Silinen veriler geçici bir önbelleğe (Cache) alınır ve kullanıcıya bir 'Toast' bildirimi ile "Geri Al" (Undo) opsiyonu sunulur.

## 🛠️ Kullanılan Teknolojiler
* **HTML5** (Semantik Yapı)
* **CSS3** (CSS Variables, Flexbox, Grid, Responsive Tasarım)
* **JavaScript** (ES6+, DOM Manipülasyonu, Clipboard API, File API)

## 📌 Kurulum & Kullanım
Proje dosyaları herhangi bir sunucu kurulumu gerektirmez. Repoyu bilgisayarınıza indirdikten sonra veya canlı önizleme linkine tıklayarak `index.html` dosyasını herhangi bir modern web tarayıcısında (Chrome, Safari, Edge) açmanız yeterlidir. Tüm veri işlemleri tarayıcınızın güvenli LocalStorage alanında gerçekleşecektir.
