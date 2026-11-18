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
- **Sonsuz radyo** — kuyruk bitmeden benzer parçalarla genişletilir; kaynak düşse de alternatifler denenir
- **Tekrar modu** — kapalı / tüm listeyi tekrarla / tek parçayı tekrarla; oynatıcıdaki döngü ikonundan değişir
- **Karışık çal** — kuyruğu karıştırır, ikon anında durumu gösterir
- **Ses kalitesi** — düşük / orta / yüksek / kayıpsız; değişimde parça aynı pozisyondan yeniden açılır
- **Arka plan çalma** — ekran kilitliyken devam eder, bildirim/kilit ekranı kontrolleri
- **Ekolayzer** — açılışta ve ayar değişiminde uygulanır, parça değişiminde kesilme yapmaz
- **Ses düzeltmeleri** — ilk oynatmada sessizlik/çizirti oluşmaz
- **Çalma listeleri** — oluşturma, adlandırma, silme ve liste içi sıralama düzenleme; sıra kalıcıdır
- **Sanatçı profilleri** — sanatçının parçaları ayrı çalma listesi olarak kaydedilir ve indirilir

### 🔎 Arama
- **Metin arama** — şarkı, sanatçı ve YouTube bağlantıları; sonuçlar önbellekte tutulur
- **Yerel Whisper sesli arama** — Google/sistem tanıma kullanılmaz; kayıt cihazda
  metne çevrilir. İlk kullanımda ~32 MB model indirilir. Mikrofon **yalnızca**
  düğmeye basıldığında açılır ve izin o anda istenir
- **Arama sonuçları** — “Çalma Listeleri ve Şarkılar” başlığı altında sanatçının
  tüm parçaları ayrı listede; “Tümünü indir” ve “Kitaplığıma kaydet” butonları
- **Kendiliğinden değişmez** — ana sayfa ve sonuçlar yalnızca yukarıdan aşağıya
  kaydırınca yenilenir; sanatçı parçaları da ancak o zaman tazelenir

### 🎨 Kişiselleştirme
- **18 vurgu rengi**, **Koyu / Açık / Sistem** teması, OLED siyah zemin
- Açık temada tüm yüzeyler ve metinler tema duyarlı paletten gelir; siyah yazı
  koyu zemin üstünde kalmaz
- **Dil** — Ayarlar'dan seçilen dil uygulamaya anında uygulanır (TR/EN tam,
  diğer diller İngilizceye düşer); sesli aramanın dili de bu ayarı izler
- Dinleme geçmişine göre kişisel ana sayfa

### ⬇️ İndirme ve oda
- Şarkılar doğrudan cihaz depolamasına kaydedilir (`Download/CloudTune`);
  itag/MIME'ye göre doğru uzantı (`.webm` / `.m4a` / `.mp3`), sanatçı ve arama
  grupları ayrı kartlarda; internet olmadan çalınabilir. Masaüstünde Belgeler
  klasörü kullanılır.
- **Odalar** — oda listesi (ad, kod, kişi sayısı, kilit), şifresiz odaya tek
  dokunuşla katılım, davet linkinde şifre (`cloudtune://room/KOD?p=...`),
  uzaktan katılımcı avatarları. Başka cihaz bilgileri kullanıcı onayına bağlıdır.
- **Kararlı avatar** — sürümlü dosya adı ve cache key'i; her çizimde değişmez.

### 🛠️ Onarım botu
Arka planda düşük kaynakla çalışır; akış, indirme ve bağlantı hatalarını sessizce
onarır. Ayarlar → **Tam onarımı çalıştır** tüm aşamaları zorla koşar ve sonucu
gösterir. Loglar yalnızca cihazda tutulur; e-posta/uzak servise veri gönderilmez.

### 🔗 Bağlantılar
Desteklenen adresler: `youtu.be`, `m.youtube.com`, `music.youtube.com`,
`youtube.com`, `www.youtube.com`. Ayarlar → **Desteklenen bağlantılar**
anahtarıyla uygulama içi açma kapatılabilir.

---

## ⬇️ İndirme

| Platform | Dosya | Not |
|---|---|---|
| Android — tüm cihazlar | `CloudTune-universal.apk` | Mimari bilmiyorsanız bunu seçin (Android 7.0+) |
| Android arm64 | `CloudTune-arm64.apk` | Çoğu modern telefon |
| Android armv7 | `CloudTune-armv7.apk` | Eski 32-bit cihazlar |
| Android x86_64 | `CloudTune-x86_64.apk` | x86 tablet / emülatör |
| Linux (deb) | `CloudTune-linux.deb` | `sudo apt install ./CloudTune-linux.deb` — `libmpv2` otomatik gelir |
| Linux (tar.gz) | `CloudTune-linux.tar.gz` | `libmpv2` kurulu olmalı: `sudo apt install libmpv2` |
| Windows | `CloudTune-windows.zip` | ⚠️ Mevcut dosya `3.0.5+206`; güncel sürüm CI ödeme limiti nedeniyle yayınlanamadı |
| iOS | `apps.json` kaynağı | ⚠️ Mevcut IPA eski; aynı CI engeli nedeniyle güncellenemedi |

Tüm dosyalar: [son sürüm](https://github.com/Arise1881/cloudtune-dist/releases/tag/cloudtune-latest)

### 3.0.41+242 —platform optimizasyonları

- **Android:** R8 + kaynak küçültme açık; ABI APK'ları 20–26 MB. HTTP trafiği
  kapalı, tüm bağlantılar HTTPS/wss. CI, özel manifest/izinleri koruyan
  commit'li `android/` dosyalarını kullanıyor.
- **Linux:** Stripped binary, `ldd` ile doğrulanan `libmpv2` bağımlılığı,
  sürüm+build numaralı deb (`3.0.41-242`), doğru `StartupWMClass`,
  `/usr/bin/cloudtune` kısayolu ve tarball içinde masaüstü dosyası.
- **Windows / iOS:** MSVC LTCG + zorunlu `flutter_windows.dll`; imzasız iOS IPA
  obfuscation ile küçültüldü. **İkili paketler CI ödeme limiti nedeniyle eski**
  kaldı; limit düzelince yenilenecek.
- **Uygulama:** Oda presence/ack senkronu, doğru kişi sayısı, avatar/discovery
  temizliği; yerel Whisper, indirme/kaydetme, sıralanabilir playlist ve TR/EN dil.

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

Dinleme geçmişi, beğeniler, çalma listeleri, avatar, indirilenler, Whisper
transkriptleri ve dil tercihi yalnızca cihazda saklanır. Ses kaydı cihazda metne
çevrilir, sunucuya gönderilmez; mikrofon yalnızca siz dokunduğunuzda açılır.
Oda durumu genel bir MQTT relay üzerinden taşınır; oda kodunu/şifresini bilmeyen
kişiler aynı kanalı dinleyebilir, bu yüzden hassas bilgi paylaşmayın. Onarım
logları cihazda kalır; e-posta veya uzak servise veri gönderilmez. PC kapalıyken
de uygulama çalışır; yerel servis bağımlılığı yoktur.

## 📄 Lisans

MIT — [kaynak depo](https://github.com/Arise1881/cloudtune)
