# Değişiklik Günlüğü (Changelog)

Bu projedeki tüm önemli değişiklikler bu dosyada belgelenmektedir.
Format [Keep a Changelog](https://keepachangelog.com/tr/1.0.0/) standardını temel alır ve sürümleme [Semantik Sürümleme](https://semver.org/lang/tr/) kurallarına uyar.

---

## [1.1.0] - 2026-11-06

### ✨ Eklenenler (Added)
- **Çift Zıplama (Double Jump)**:
  - Karakter havadayken ikinci bir zıplama hakkı kazandı (`jumpCount < maxJumps`).
  - Çift zıplama anına özel genişleyen neon halka parçacık efekti eklendi.
  - Web Audio API ile sentezlenen özel çift zıplama ses efekti (`playDoubleJumpSound`).
- **Eğilme & Kayma Mekaniği (Duck & Slide)**:
  - `S` ve `Aşağı Ok (↓)` tuşları ile karaktere eğilme/kayma hareketi kazandırıldı.
  - Karakter eğildiğinde boyutu aerodinamik form alarak 45px'ten 24px'e düşer.
  - Havada eğilme tuşuna basıldığında yere hızlı iniş (fast-fall) mekaniği eklendi.
  - Kayma süresince geriye doğru sürtünme toz parçacıkları ve kayma ses efekti (`playSlideSound`).
- **Altından Geçilen Uçan Engeller (Flying Siber Drones)**:
  - Yerden yüksekte asılı duran yeni uçan engel tipi (`type: 3`) eklendi.
  - Zıplayınca çarpışılan, altından yalnızca eğilerek güvenle geçilebilen 40 piksellik koridor oluşturuldu.
  - Kanat çırpma animasyonu, kırmızı sensör gözü ve zemin lazer izi eklendi.
- **Altın Toplama & Ödül Sistemi (Coins / Collectibles)**:
  - Zemin, orta yükseklik ve çift zıplamayla ulaşılan yüksek konumlarda altınlar (`Coin`) eklendi.
  - Uçan engellerin tam altına, eğilerek geçmeyi ödüllendiren altın yerleşimleri yapıldı.
  - Her altın için `+25 Puan`, altın sayacı artışı ve ekranda uçuşan `+25 🪙` yazısı eklendi.
  - Web Audio API ile kristal netliğinde altın toplama "ting" sesi (`playCoinSound`).
- **Dinamik Gece - Gündüz Döngüsü (Day-Night Cycle)**:
  - Gündüz ☀️ -> Gün Batımı 🌇 -> Yıldızlı Gece ve Ay 🌙 -> Şafak 🌄 renk interpolasyonları eklendi.
  - Gece olduğunda parıldayan 45 adet yıldız ve yumuşak hilal ay gökyüzünde belirecek şekilde kodlandı.
  - Gökyüzü döngüsüne göre değişen bulut geçirgenliği ve dağ silüeti renkleri.
- **Arayüz ve Dokunmatik Kontroller**:
  - Skor tahtasına `🪙 Altın: 0` sayacı entegre edildi.
  - Ekran altına mobilde de oynamayı sağlayan `Zıpla` ve `Eğil (Tut)` dokunmatik butonları eklendi.
  - Oyun sonu ekranında toplanan toplam altın miktarı listelendi.

### 🔄 Güncellenenler (Changed)
- `index.html` dosyası yeni mekanikleri (çift zıplama, eğilme, altınlar, gece/gündüz, uçan dronlar) kapsayacak şekilde güncellendi.
- `README.md` dokümantasyonu yeni kontroller ve oynanış ipuçlarıyla güncellendi.
- Çarpışma kutusu (hitbox) kontrolleri karakterin ayakta ve eğilme boyutlarına göre dinamik olarak uyarlandı.

---

## [1.0.0] - 2026-11-06

### ✨ İlk Sürüm (Initial Release)
- HTML5 Canvas & saf Vanilla JS ile geliştirilen sonsuz koşu & zıplama oyunu.
- Web Audio API ile zıplama, skor ve çarpışma sesleri.
- Kaktüs, yüksek kaya ve dikenli engeller.
- `localStorage` üzerinde çalışan en yüksek skor kaydı.
