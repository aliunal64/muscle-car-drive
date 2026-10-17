# Muscle Car - Open World Drive

> Çizimden tarayıcıya: Kağıt üzerinde çizilen klasik bir muscle car, Three.js ile gerçekçi bir açık dünya sürüş deneyimine dönüştürüldü.

## 📄 Proje Hakkında

Bu proje, bir kağıt üzerine çizilen basit araba eskizinin **AI prompt** ile gerçekçi bir oyun görseline, ardından **Three.js** kullanılarak tamamen oynanabilir bir tarayıcı oyununa dönüştürülmesini göstermektedir.

**Geliştirme süreci:**

\`\`\`
✏️ Kağıt çizimi → 🤖 AI görsel üretimi → 💻 Three.js 3D oyun
\`\`\`

## ✨ Özellikler

- 🏙️ **Prosedürel şehir** — Rastgele oluşturulan gökdelenler, sokaklar ve kaldırımlar
- 🌅 **Gün batımı atmosferi** — Gradient gökyüzü, dinamik ışıklandırma, yanan pencere detayları
-  **Detaylı araba modeli** — Anten, kaput hava girişleri, krom tamponlar, 5 kollu jantlar, egzoz boruları
- 💨 **Fizik motoru** — Hızlanma, frenleme, drift, el freni, lastik dumanı parçacıkları
- 🎥 **3 kamera modu** — Uzak 3. şahıs, yakın takip, kaput içi görünüm
- 🗺️ **Mini harita** — Gerçek zamanlı konum takibi
- 📊 **HUD** — Hız göstergesi (km/h), vites bilgisi, koordinatlar
- 🎨 **AAA kalitesinde grafikler** — ACES filmik ton eşleme, PCF yumuşak gölgeler, sRGB renk uzayı

## 🎮 Kontroller

| Tuş | İşlev |
|-----|-------|
| \`W\` / \`↑\` | Gaz |
| \`S\` / \`↓\` | Fren / Geri vites |
| \`A\` / \`←\` | Sola dön |
| \`D\` / \`→\` | Sağa dön |
| \`Space\` | El freni (drift) |
| \`C\` | Kamera modunu değiştir |
| \`R\` | Başlangıç noktasına sıfırla |

## 🚀 Hızlı Başlangıç

\`index.html\` dosyasını çift tıklayarak herhangi bir tarayıcıda açabilirsiniz.

## 🛠️ Teknik Detaylar

| Teknoloji | Açıklama |
|-----------|----------|
| **Three.js r128** | 3D render motoru |
| **WebGL** | GPU hızlandırmalı grafik |
| **Vanilla JS** | Harici kütüphane gerektirmez |
| **Prosedürel üretim** | Şehir ve binalar kod ile oluşturulur |
| **Canvas API** | Gökyüzü dokusu ve mini harita |

### Performans
- **Gölge haritası:** 2048×2048 PCF Soft
- **Ton eşleme:** ACES Filmic
- **Çizim mesafesi:** 2000 birim
- **Kare hızı:** 60 FPS hedefi (delta time ile stabilize)

## 📁 Proje Yapısı

\`\`\`
muscle-car-drive/
├── index.html        # Ana oyun dosyası (tek dosya, bağımlılık yok)
└── README.md         # Bu dosya
\`\`\`

> 💡 Tüm oyun tek bir HTML dosyasında çalışır — harici asset, resim veya kütüphane indirmeye gerek yoktur (Three.js CDN üzerinden yüklenir).


##  Katkıda Bulunma

Pull request ve issue'lar için geliştirme önerileri:
- [ ] Daha fazla araba modeli
- [ ] NPC trafik sistemi
- [ ] Ses efektleri (motor, lastik)
- [ ] Gece/gündüz döngüsü
- [ ] Çarpışma fiziği
