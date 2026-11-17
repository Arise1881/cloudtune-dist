<p align="center">
  <img src="https://raw.githubusercontent.com/Arise1881/cloudtune-dist/main/icon.png" width="120" height="120" alt="CloudTune">
  <h1 align="center">🎵 CloudTune</h1>
  <p align="center"><b>Açık kaynak, YouTube destekli, reklamsız müzik çalar</b></p>
  <p align="center">
    <a href="#-indirme"><img src="https://img.shields.io/badge/indir-APK%20%2F%20DEB%20%2F%20IPA-1DB954?style=flat-square"></a>
    <a href="https://raw.githubusercontent.com/Arise1881/cloudtune-dist/main/update.json"><img src="https://img.shields.io/badge/güncelleme-OTA-9C27B0?style=flat-square"></a>
    <a href="https://github.com/Arise1881/cloudtune"><img src="https://img.shields.io/badge/kaynak-kod-1E88E5?style=flat-square"></a>
  </p>
</p>

**CloudTune**, şarkıları doğrudan cihazdan YouTube üzerinden arayıp çalan,
reklamsız ve açık kaynak bir müzik uygulamasıdır. Güncel sürüm Android 7.0+
ve Linux için yayında. Linux oynatma motoru `media_kit + libmpv`'dir; `deb`
paketi `libmpv2`'yi otomatik kurar. Windows/iOS kaynak ve CI hazır; mevcut
paketler eski, GitHub billing/spending limiti düzeltildikten sonra yenilenecek.
Hesap, abonelik veya PC sunucusu gerekmez.

Güncel sürüm ve indirme bağlantıları: **`update.json`** — uygulama içi
güncelleme de bu dosyayı okur.

---

## ✨ Özellikler

### 🎧 Çalma
- **Doğrudan YouTube** — aracı sunucu yok, arama ve akış cihazda çözülür
- **Sonsuz radyo** — kuyruk bitince benzer parçalarla devam eder
- **Arka plan çalma** — ekran kilitliyken devam eder, bildirim/kilit ekranı kontrolleri
- **Ekolayzer** — açılışta ve ayar değişiminde uygulanır, parça değişiminde kesilme yapmaz
- **Ses düzeltmeleri** — ilk oynatmada sessizlik/çizirti oluşmaz
- **Çalma listeleri** — tek kaydırmalı liste, “Tümünü çal”
- **Sanatçı profilleri** — sanatçının tüm parçaları tek listede

### 🔎 Arama
- **Metin arama** — şarkı, sanatçı ve YouTube bağlantıları
- **Sesli arama** — mikrofona dokununca açılır, konuşma bitince veya basılı tutup
  bırakınca arar; uygulama sürekli mikrofonu dinlemez
- **Arama sonuçları** — “Çalma Listeleri ve Şarkılar” başlığı altında sanatçının
  tüm parçaları, ayrı “Arama Sonuçları” bölümü
- **Kendiliğinden değişmez** — ana sayfa ve sonuçlar yalnızca yukarıdan aşağıya
  kaydırınca yenilenir

### 🎨 Kişiselleştirme
- **18 vurgu rengi**, **Koyu / Açık / Sistem** teması, OLED siyah zemin
- Açık temada tüm yüzeyler ve metinler tema duyarlı paletten gelir; siyah yazı
  koyu zemin üstünde kalmaz
- Dinleme geçmişine göre kişisel ana sayfa

### ⬇️ İndirme ve oda
- Şarkılar doğrudan cihaz depolamasına kaydedilir (`Download/CloudTune`);
  internet olmadan çalınabilir. Masaüstünde Belgeler klasörü kullanılır.
- **Oda** — oda koduyla paylaşım, avatar ve beğeniler (MQTT)

### 🛠️ Onarım botu
Arka planda düşük kaynakla çalışır; akış hatalarını sessizce onarır. Sıralama:
doğrudan YouTube (yerel InnerTube) → tekrar deneme → anonim cihaz raporu
(`CloudTune@hotmail.com`). Kullanıcıya ham hata mesajı gösterilmez.

### 🔗 Bağlantılar
Desteklenen adresler: `youtu.be`, `m.youtube.com`, `music.youtube.com`,
`youtube.com`, `www.youtube.com`. Ayarlar → **Desteklenen bağlantılar**
anahtarıyla uygulama içi açma kapatılabilir.

---

## ⬇️ İndirme

| Platform | Dosya | Not |
|---|---|---|
| Android — tüm cihazlar | `CloudTune-universal.apk` | Miminari bilmiyorsanız bunu seçin (Android 7.0+) |
| Android arm64 | `CloudTune-arm64.apk` | Çoğu modern telefon |
| Android armv7 | `CloudTune-armv7.apk` | Eski 32-bit cihazlar |
| Android x86_64 | `CloudTune-x86_64.apk` | x86 tablet / emülatör |
| Linux (deb) | `CloudTune-linux.deb` | `sudo apt install ./CloudTune-linux.deb` — `libmpv2` otomatik gelir |
| Linux (tar.gz) | `CloudTune-linux.tar.gz` | `libmpv2` kurulu olmalı: `sudo apt install libmpv2` |
| Windows | `CloudTune-windows.zip` | ⚠️ Mevcut dosya `3.0.5+206`; güncel sürüm CI ödeme limiti nedeniyle yayınlanamadı |
| iOS | `apps.json` kaynağı | ⚠️ Mevcut IPA eski; aynı CI engeli nedeniyle güncellenemedi |

Tüm dosyalar: [son sürüm](https://github.com/Arise1881/cloudtune-dist/releases/tag/cloudtune-latest)

### İlk kurulum
1. Dosyayı indirin; Android'de **Bilinmeyen kaynaklardan yükleme** iznini verin.
2. APK'yı kurun ve uygulamayı açın.
3. Bildirim iznini verin (arka plan çalma için); mikrofon izni yalnızca sesli
   arama düğmesine bastığınızda istenir.
4. Ayarlar → **Tema**'dan açık/koyu/sistem modunu ve vurgu rengini seçin.
5. Arama kutusuna şarkı yazın veya YouTube bağlantısı yapıştırın. İçerik
   kendiliğinden değişmez; yenilemek için yukarıdan aşağıya kaydırın.

### Cihaz uyumu

| Android | API | Destek |
|---|---|---|
| 7.0 – 7.1 | 24 – 25 | ✅ (`minSdk 24`) |
| 8 – 10 | 26 – 29 | ✅ |
| 11 – 14 | 30 – 34 | ✅ |
| 15+ | 35+ | ✅ (`targetSdk 36`) |

`arm64-v8a`, `armeabi-v7a`, `x86_64` ayrı paketler; bilinmeyen mimaride
`CloudTune-universal.apk` kullanılır. Uygulama güncelleyicisi cihazın ABI'sini
algılar ve uygun paketi indirir. Telefon, tablet, katlanabilir ve geniş ekran
cihazlar desteklenir (`supports-screens`, `resizeableActivity`).

---

## 🔄 Güncelleme

Uygulama açılışta `update.json` dosyasını okur; yeni sürüm varsa ana sayfada
bildirim çıkar. İndirilen APK cihazın ABI'sine göre seçilir (arm64 / armv7 /
x86_64 / evrensel). Kurulum için “Bilinmeyen kaynaklardan yükleme” izni gerekir.

Manifest iki adresten erişilebilir:

- Raw (her zaman güncel): `https://raw.githubusercontent.com/Arise1881/cloudtune-dist/main/update.json`
- GitHub Pages (CDN önbellekli): `https://arise1881.github.io/cloudtune-dist/update.json`

## 📁 Bu depodaki dosyalar

| Dosya | Açıklama |
|---|---|
| `README.md` | Bu sayfa — indirme, kurulum, uyum, güncelleme, gizlilik |
| `index.html` | GitHub Pages indirme portalı (sürüm kartları, QR kodlar) |
| `update.json` | Uygulama içi güncelleyicinin okuduğu OTA manifest |
| `apps.json` | AltStore / SideStore için iOS kaynak manifesti |
| `icon.png` | Uygulama ikonu (Pages ve Linux masaüstü girişi) |
| `header.png` | Pages başlık görseli |
| `apk-qr.png` | Android indirme QR kodu |
| `ipa-qr.png` | iOS kaynak QR kodu |
| `sidestore-qr.png` | SideStore kurulum QR kodu |
| `video-poster.png` | Pages video kapak görseli |
| `tunnel.txt` | Cloudflare tünel / altyapı notu |

Kurulabilir dosyalar depoda değil,
[son sürüm](https://github.com/Arise1881/cloudtune-dist/releases/tag/cloudtune-latest)
asset'lerinde tutulur: `CloudTune-arm64.apk`, `CloudTune-armv7.apk`,
`CloudTune-x86_64.apk`, `CloudTune-universal.apk`, `CloudTune-linux.deb`,
`CloudTune-linux.tar.gz`, `CloudTune-windows.zip`, `CloudTune.ipa`.

---

## 🔐 Gizlilik

Dinleme geçmişi, beğeniler, çalma listeleri, avatar ve tercihler yalnızca
cihazda saklanır. Sunucuya gönderilen tek veri, çözülemeyen bir akış hatasında
gönderilen anonim cihaz raporudur (platform, sürüm, video kimliği). PC kapalıyken
de uygulama çalışır; yerel servis bağımlılığı yoktur.

## 📄 Lisans

MIT — [kaynak depo](https://github.com/Arise1881/cloudtune)
