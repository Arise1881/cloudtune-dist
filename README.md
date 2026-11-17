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
reklamsız ve açık kaynak bir müzik uygulamasıdır. Android 5.0+, Linux, Windows
ve iOS'ta (AltStore/SideStore) çalışır. Hesap, abonelik veya PC sunucusu gerekmez.

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
| Android — tüm cihazlar | `CloudTune-universal.apk` | Miminari bilmiyorsanız bunu seçin (Android 5.0+) |
| Android arm64 | `CloudTune-arm64.apk` | Çoğu modern telefon |
| Android armv7 | `CloudTune-armv7.apk` | Eski 32-bit cihazlar |
| Android x86_64 | `CloudTune-x86_64.apk` | x86 tablet / emülatör |
| Linux (deb) | `CloudTune-linux.deb` | `sudo apt install ./CloudTune-linux.deb` |
| Linux (tar.gz) | `CloudTune-linux.tar.gz` | Dağıtımdan bağımsız |
| Windows | `CloudTune-windows.zip` | Zip'i açıp `cloudtune.exe` |
| iOS | `apps.json` kaynağı | AltStore/SideStore ile ekleyin |

Tüm dosyalar: [son sürüm](https://github.com/Arise1881/cloudtune-dist/releases/tag/cloudtune-latest)

### İlk kurulum
1. Dosyayı indirin; Android'de **Bilinmeyen kaynaklardan yükleme** iznini verin.
2. APK'yı kurun ve uygulamayı açın.
3. Bildirim iznini verin (arka plan çalma için); mikrofon izni yalnızca sesli
   arama düğmesine bastığınızda istenir.
4. Ayarlar → **Tema**'dan açık/koyu/sistem modunu ve vurgu rengini seçin.
5. Arama kutusuna şarkı yazın veya YouTube bağlantısı yapıştırın. İçerik
   kendiliğinden değişmez; yenilemek için yukarıdan aşağıya kaydırın.

---

## 🔄 Güncelleme

Uygulama açılışta `update.json` dosyasını okur; yeni sürüm varsa ana sayfada
bildirim çıkar. İndirilen APK cihazın ABI'sine göre seçilir (arm64 / armv7 /
x86_64 / evrensel). Kurulum için “Bilinmeyen kaynaklardan yükleme” izni gerekir.

Manifest iki adresten erişilebilir:

- Raw (her zaman güncel): `https://raw.githubusercontent.com/Arise1881/cloudtune-dist/main/update.json`
- GitHub Pages (CDN önbellekli): `https://arise1881.github.io/cloudtune-dist/update.json`

---

## 🔐 Gizlilik

Dinleme geçmişi, beğeniler, çalma listeleri, avatar ve tercihler yalnızca
cihazda saklanır. Sunucuya gönderilen tek veri, çözülemeyen bir akış hatasında
gönderilen anonim cihaz raporudur (platform, sürüm, video kimliği). PC kapalıyken
de uygulama çalışır; yerel servis bağımlılığı yoktur.

## 📄 Lisans

MIT — [kaynak depo](https://github.com/Arise1881/cloudtune)
