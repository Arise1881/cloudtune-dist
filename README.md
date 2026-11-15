<p align="center">
  <img src="https://raw.githubusercontent.com/Arise1881/cloudtune-dist/main/icon.png" width="120" height="120" alt="CloudTune">
  <h1 align="center">🎵 CloudTune</h1>
  <p align="center"><b>Açık kaynak, YouTube destekli müzik çalar</b></p>
  <p align="center">
    <a href="#-indirme"><img src="https://img.shields.io/badge/indir-APK%20%2F%20DEB%20%2F%20IPA-1DB954?style=flat-square"></a>
    <a href="https://raw.githubusercontent.com/Arise1881/cloudtune-dist/main/update.json"><img src="https://img.shields.io/badge/güncelleme-OTA-9C27B0?style=flat-square"></a>
    <a href="../cloudtune"><img src="https://img.shields.io/badge/kaynak-kod-1E88E5?style=flat-square"></a>
  </p>
</p>

**CloudTune**, şarkıları doğrudan YouTube üzerinden arayıp çalan, reklamsız ve
açık kaynak bir müzik uygulamasıdır. Android, Linux ve Windows'ta çalışır;
iOS derlemesi AltStore kaynağı üzerinden dağıtılır.

Güncel sürüm ve indirme bağlantıları: **`update.json`** (uygulama içi
güncelleme de bu dosyayı okur).

---

## ✨ Özellikler

### 🎧 Çalma
- **Doğrudan YouTube** — aracı sunucu yok, akış doğrudan cihaza gelir
- **Sonsuz radyo** — kuyruk bitince benzer parçalarla devam eder
- **Arka plan çalma** — ekran kilitliyken devam eder
- **Kilit ekranı / bildirim kontrolleri** — şarkı bilgisi, ileri-geri, beğen
- **Çalma listeleri** — tek kaydırmalı liste, tümünü çal
- **Sanatçı profilleri** — sanatçının tüm parçaları tek listede
- **Oda** — kendi avatarını yükle, beğendiğin parçaları tek yerde topla

### 🔗 Bağlantılar
Desteklenen dört adres: `youtu.be`, `m.youtube.com`, `youtube.com`,
`www.youtube.com`. Ayarlar'daki **Desteklenen bağlantılar** anahtarıyla
uygulama içi açma kapatılabilir.

### 🛠️ Onarım botu
Arka planda düşük kaynakla çalışır; akış hatalarını sessizce onarır.
Sıralama: doğrudan YouTube → Cloudflare yedek akışı → cihaz raporu
(`CloudTune@hotmail.com`). Kullanıcıya hata mesajı gösterilmez.

### ⬇️ İndirme
Şarkılar doğrudan cihaz depolamasına kaydedilir
(`Download/CloudTune`). Masaüstünde belgeler klasörüne yazılır.

### 🎨 Kişiselleştirme
18 vurgu rengi, dinleme geçmişine göre kişisel ana sayfa, OTA güncelleme.

---

## ⬇️ İndirme

| Platform | Dosya |
|---|---|
| Android (arm64) | `CloudTune-arm64.apk` |
| Android (armv7) | `CloudTune-armv7.apk` |
| Android (x86_64) | `CloudTune-x86_64.apk` |
| Android (evrensel) | `CloudTune-universal.apk` |
| Linux (deb) | `CloudTune-linux.deb` |
| Linux (tar.gz) | `CloudTune-linux.tar.gz` |
| Windows | `CloudTune-windows.zip` |
| iOS (AltStore) | `apps.json` kaynağı |

Tüm dosyalar: [son sürüm](https://github.com/Arise1881/cloudtune-dist/releases/tag/cloudtune-latest)

---

## 🔄 Güncelleme

Uygulama açılışta `update.json` dosyasını okur; yeni sürüm varsa ana sayfada
bildirim çıkar ve APK'yı indirip kurulumu başlatır.

## 🔐 Gizlilik

Dinleme geçmişi, beğeniler ve avatar yalnızca cihazda saklanır. Sunucuya
gönderilen tek veri, çözülemeyen bir akış hatasında gönderilen anonim cihaz
raporudur (platform, sürüm, video kimliği).

## 📄 Lisans

MIT
