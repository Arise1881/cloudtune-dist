<p align="center">
  <img src="https://raw.githubusercontent.com/Arise1881/melody-dist/main/icon.png" width="120" height="120" alt="Melody">
  <h1 align="center">🎵 Melody</h1>
  <p align="center"><b>Spotify temalı, açık kaynak, YouTube destekli müzik çalar</b></p>
  <p align="center">
    <a href="#✨-özellikler"><img src="https://img.shields.io/badge/özellikler-40%2B-1DB954?style=flat-square"></a>
    <a href="#⬇️-indirme"><img src="https://img.shields.io/badge/sürüm-2.1.6%20(33)-1E88E5?style=flat-square"></a>
    <a href="#-çevrimiçi-güncelleme"><img src="https://img.shields.io/badge/güncelleme-OTA-9C27B0?style=flat-square"></a>
    <a href="LICENSE"><img src="https://img.shields.io/badge/lisans-MIT-1DB954?style=flat-square"></a>
  </p>
</p>

> **Melody**: milyonlarca şarkıyı arayıp çalan, indiren, **arka planda kesintisiz** dinleten,
> premium arayüzlü açık kaynak müzik uygulaması. Android, iOS, Linux ve Windows 11 destekli.

**Sürüm:** 2.1.6 (build 33) · **Yayın:** `melody-latest`

---

## ✨ Özellikler

### 🖤 Çalma
- ✅ **Sonsuz otomatik çalma** — şarkı biter, benzer şarkılar hiç susmadan gelir
- ✅ **Arka plan çalma** — ekran kilitli / uygulama kapalıyken devam eder
- ✅ **Kilit ekranı + bildirim kontrolleri** (play / pause / ileri / geri)
- ✅ **Oynatma hızı** — 0.5x – 2x (6 kademe, kalıcı)
- ✅ **Crossfade** — 2–10 sn yumuşak geçiş (ayarlanabilir)
- ✅ **Karıştır / Tekrar**, **oturum kaldırma** (kapatılan şarkı aynı konumdan döner)
- ✅ **Akıllı ön-çözümleme** — sıradaki şarkı şarkı bitmeden hazırlanır → anında geçiş

### 🎛 Ses
- ✅ **5 kalite kademesi** — Auto / Ultra (lossless) / Yüksek 320kbps / Orta / Düşük
- ✅ **7 bant ekolayzer** — Flat, Pop, Rock, Jazz, Klasik, Bas, Vokal
- ✅ Ses **asla transkode edilmez**; platforma göre en iyi akış otomatik seçilir

### 📚 Kitaplık
- ✅ Canlı arama + son aramalar
- ✅ Çevrimdışı indirmeler (ilerleme + boyut takibi)
- ✅ Favoriler · çalma listeleri (oluştur/adlandır/sil) · dinleme geçmişi
- ✅ Şarkı radyosu · şarkı sözleri (eş zamanlı vurgulu) · sanatçı sayfaları
- ✅ Sıralama (queue) görünümü — sırala, kaldır, yeniden düzenle

### 🌍 Bağlantı
- ✅ **Oda sistemi** — kodla katıl, senkronize dinle
- ✅ **Manuel çevrimdışı mod** — yalnızca indirilenler
- ✅ **OTA güncelleme** — açılışta otomatik kontrol, tek dokunuşla kurulum
- ✅ **Uyku zamanlayıcısı** — 5dk – 1sa

### 🎨 Arayüz
- ✅ Karanlık / Açık tema · 5 vurgu rengi (Yeşil, Mavi, Mor, Kırmızı, Turuncu)
- ✅ Trend ana sayfa (küratörlü yatay akış) · mini oynatıcı · dinamik arka plan

## ⚙️ Varsayılan Ayarlar
- **Müzik Kalitesi:** Uygulama açıldığında otomatik olarak **Ultra (lossless)** kalitede çalınır. Daha düşük kalite tercih ederseniz ayarlarından değiştirebilirsiniz.
- **Çevrimdışı Başlangıç:** Uygulama ilk açıldığında veya internet kesildiğinde, önceki oturumda indirilen şarkıdan devam eder. Yeni şarkı araması yapmadan mevcut indirilen listesini kullanır.

---

## ⬇️ İndirme

### Android

| Dosya | Boyut | Link |
|---|---|---|
| Melody.apk (arm64 — önerilir) | 21 MB | [**İndir**](https://github.com/Arise1881/melody-dist/releases/download/melody-latest/Melody.apk) |
| Melody-universal.apk (tüm cihazlar) | 60 MB | [**İndir**](https://github.com/Arise1881/melody-dist/releases/download/melody-latest/Melody-universal.apk) |

> Kurulum: APK'yı indir → aç → izin ver → kur. Açılırken "Bilinmeyen kaynak" izni istenebilir.
> 📱 <img src="https://raw.githubusercontent.com/Arise1881/melody-dist/main/apk-qr.png" width="64" align="center"> QR ile doğrudan telefonda indirme için de bu görsele bakabilirsin.

### iPhone / iPad

| Dosya | Link |
|---|---|
| Melody.ipa | [**İndir**](https://github.com/Arise1881/melody-dist/releases/download/melody-latest/Melody.ipa) |

Apple `.ipa` dosyalarının doğrudan kurulmasına izin vermez; 3 yol:

- **A (önerilen, PC gerekmez) — SideStore:**
  1. **iOS 27+:** tarayıcıdan [SideInstaller](https://frizzlem.github.io/SideInstaller) → uygulamayı kur → **Install SideStore** · **iOS 26 ve altı:** [AppleJr](https://applejr.net) ile **ESign** kur, SideStore IPA'sını cihazdan imzala
  2. SideStore → **Settings → Sources** → ekle:
     `altstore://source?url=https://raw.githubusercontent.com/Arise1881/melody-dist/main/apps.json`
  3. Kaynaktan **Melody** → **Install** → Apple ID onayı ✅
  4. 7 günlük imza yenilemesi WiFi ile otomatik yapılır
- **C: AltStore** → aynı kaynak linkini telefonda aç → listeden Melody → **Install** (ilk kurulumda tek seferlik bilgisayar).
- **D: Sideloadly (Windows/Mac + USB)** → [sideloadly.io](https://sideloadly.io) → IPA'yı pencereye sürükle → Apple ID → Start.

> iOS 16+ ilk kurulumda: Ayarlar → Gizlilik ve Güvenlik → **Geliştirici Modu** aç.
> iOS 14–16.6.1/17.0 TrollStore kullanıcıları: IPA'yı TrollStore ile aç.

### Linux Mint / Ubuntu / Debian

| Dosya | Link |
|---|---|
| `.deb` | [**melody_2.2.0_amd64.deb indir**](https://github.com/Arise1881/melody-dist/releases/download/melody-latest/melody_2.2.0_amd64.deb) |
| Taşınabilir tar.gz | [**Melody-linux.tar.gz indir**](https://github.com/Arise1881/melody-dist/releases/download/melody-latest/Melody-linux.tar.gz) |

```bash
sudo apt install ./melody_2.2.0_amd64.deb   # menüde "Melody" görünür
# veya
tar -xzf Melody-linux.tar.gz && ./bundle/melody
```

### Windows 11

| Dosya | Link |
|---|---|
| `Melody-windows.zip` (x64) | [**İndir**](https://github.com/Arise1881/melody-dist/releases/download/melody-latest/Melody-windows.zip) |

Kurulum, 3 adım:

1. ZIP'i yukarıdaki **İndir** butonuyla al (henüz listede yoksa, yayın sürecinde üretilir — birkaç dakika sonra tekrar kontrol et).
2. ZIP'i çıkart → `melody.exe` dosyasını çalıştır.
3. İlk açılışta Windows "Korumalı" (SmartScreen) uyarısı verebilir → **Yine de Çalıştır**. Uygulama kurulum gerektirmez; klasörü nereye istersen oraya taşı.

Kurulum istemiyorsan kaynaktan derle: **Flutter SDK + Visual Studio 2022 (C++ masaüstü geliştirme iş yükü)** kur → `flutter build windows --release` → `build\windows\x64\runner\Release\melody.exe`.

---

## 📲 Çevrimiçi Güncelleme (OTA)

Bu sayfanın `update.json` dosyası Pages üzerinden sunulur:

```
https://arise1881.github.io/melody-dist/update.json
```

1. Uygulama açıldığında manifest kontrol edilir (varsayılan 10dk önbellek).
2. Yeni sürüm varsa banner görünür → **İndir + Kur**.
3. Güncelleme ayrı oturumda tamamlanır; müzik ve veriler etkilenmez.

> Sürüm eskiliği: 2.1.5 ve altı → kullanıcı otomatik 2.1.6'ya güncellenir.

---

## 🏗 Yansıtılan Yapı

```
melody-dist/            ← bu yayın reposu (manifest + indirmeler)
├── update.json         OTA manifest (sürüm/code/URL'ler)
├── apps.json           AltStore kaynağı (iOS)
├── index.html          GitHub Pages tanıtım sayfası
├── icon.png / header.png / apk-qr.png / ipa-qr.png
└── README.md           ← kurulum rehberi
```

## ⚖️ Yasal

Açık kaynak, tamamen kişisel kullanım. Uygulama hiçbir içeriği barındırmaz;
indirilen içeriklerin kullanımından geliştirici sorumlu değildir, telif haklarına uyun.

## 📄 Lisans

MIT