🏝️ Antalya Rota Asistanı (Full-Stack)
Antalya'yı keşfetmek isteyenler için geliştirilmiş; Yapay Zeka (AI) destekli, anlık Hava Durumu entegrasyonlu ve dinamik rota oluşturma özellikli modern bir web rehberi.

Bu proje, turistlerin Tarih, Doğa, Eğlence, Dalış, Tekne ve Yemek kategorilerinde en iyi mekanları bulmasını, kişisel favori listelerini oluşturmasını ve Google Gemini AI sayesinde o anki hava durumuna göre kişiselleştirilmiş gezi tavsiyeleri almasını sağlar.

🚀 Özellikler
🗺️ Kategori Bazlı Keşif: Tarihi yerlerden gizli koylara, restoranlardan dalış noktalarına kadar 6 farklı kategoride filtreleme.

🤖 AI Destekli Rehber (Gemini): "AI İpucu" butonu ile mekanın o anki hava durumunu analiz eder ve turist rehberi ağzıyla size özel tavsiye verir.

☀️ Gerçek Zamanlı Hava Durumu: OpenWeatherMap API kullanılarak her mekanın anlık sıcaklık ve durum bilgisi çekilir.

❤️ Favoriler ve Rota Çizme: Beğendiğiniz mekanları listeye ekleyip, tek tıkla Google Maps üzerinde optimize edilmiş rota oluşturabilirsiniz.

💳 Dinamik Fiyatlandırma: "Müzekart Var/Yok" seçeneği ile giriş ücretlerini anında günceller.

💬 Gerçek Yorumlar: Yemek mekanları için doğrudan Google Maps yorumlarına giden hızlı bağlantılar.

📱 Modern Arayüz: Oval butonlar, yumuşak geçişler (smooth scroll) ve duyarlı (responsive) tasarım.

🛠️ Kullanılan Teknolojiler
Frontend (İstemci)
React.js: Bileşen tabanlı modern UI.

Google Generative AI SDK: Gemini modeline bağlanmak için.

CSS3: Flexbox/Grid yapısı, Backdrop-filter efektleri ve Smooth Scroll.

Backend (Sunucu)
Node.js & Express.js: REST API yapısı.

Axios: Harici API (OpenWeather) istekleri için.

Dotenv: API anahtarlarını güvenli saklamak için.

CORS: Frontend ve Backend arası güvenli iletişim.

⚙️ Kurulum ve Çalıştırma
Projeyi yerel bilgisayarınızda çalıştırmak için aşağıdaki adımları izleyin.

1. Projeyi Klonlayın
Bash
git clone https://github.com/KULLANICI_ADIN/antalya-rota-asistani.git
cd antalya-rota-asistani
2. Backend (Sunucu) Kurulumu
Backend klasörüne gidin, paketleri yükleyin ve sunucuyu başlatın.

Bash
cd backend
npm install
⚠️ Önemli: backend klasörü içinde .env adında bir dosya oluşturun ve içine OpenWeatherMap API anahtarınızı ekleyin:

Kod snippet'i
WEATHER_API_KEY=senin_openweathermap_api_keyin
Sunucuyu başlatın:

Bash
node server.js
(Backend http://localhost:5000 adresinde çalışacaktır.)

3. Frontend (Arayüz) Kurulumu
Yeni bir terminal açın, frontend klasörüne gidin ve paketleri yükleyin.

Bash
cd ../frontend
npm install
⚠️ Önemli: frontend klasörü içinde .env adında bir dosya oluşturun ve Google Gemini API anahtarınızı ekleyin:

Kod snippet'i
REACT_APP_GEMINI_KEY=senin_gemini_api_keyin
Uygulamayı başlatın:

Bash
npm start
(Uygulama http://localhost:3000 adresinde açılacaktır.)

📸 Ekran Görüntüleri
(Buraya uygulamanın ekran görüntülerini ekleyebilirsin. Örneğin: ![Uygulama Ana Sayfa](./screenshots/home.png))

📂 Proje Yapısı
Plaintext
Antalya-Rota-Asistani/
├── backend/
│   ├── server.js        # API endpointleri ve sunucu ayarları
│   ├── .env             # Hava durumu API anahtarı (Gizli)
│   └── package.json
│
└── frontend/
    ├── public/
    ├── src/
    │   ├── App.js       # Ana uygulama mantığı ve UI
    │   └── index.js
    ├── .env             # Gemini AI API anahtarı (Gizli)
    └── package.json
🤝 Katkıda Bulunma
Bu repoyu Fork'layın.

Yeni bir özellik dalı (branch) oluşturun (git checkout -b yeni-ozellik).

Değişikliklerinizi Commit edin (git commit -m 'Yeni özellik eklendi').

Branch'inizi Push edin (git push origin yeni-ozellik).

Bir Pull Request oluşturun.

📄 Lisans
Bu proje MIT lisansı ile lisanslanmıştır.
