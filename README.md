# 🎮 Zıplama Macerası (Jump Runner)

HTML5 Canvas ve saf JavaScript ile geliştirilmiş, harici kütüphane gerektirmeyen klasik sonsuz koşu & zıplama oyunu.

## ✨ Özellikler
- **Saf Web Teknolojisi**: Harici hiçbir kütüphane/paket gerekmez (`HTML5 Canvas`, `Vanilla JS`, `CSS3`).
- **Dinamik Ses Efektleri**: Web Audio API kullanılarak üretilen zıplama, skor ve çarpışma sesleri (harici ses dosyası indirilmesi gerekmez).
- **Akıcı Animasyonlar**: Zıplama ve inişlerde squish & stretch deformasyonları, toz ve çarpışma parçacık efektleri.
- **Kademeli Zorluk**: Skor yükseldikçe oyun hızı tatlı bir tempoda artar.
- **Yüksek Skor Kaydı**: En yüksek skor tarayıcı hafızasında (`localStorage`) saklanır.
- **Mobil & Dokunmatik Uyumlu**: Hem klavye hem fare/dokunmatik tıklamaları destekler.

## 🕹️ Kontroller
- **Zıplama / Başlatma / Yeniden Başlatma**: `Space` veya `Yukarı Ok (↑)` tuşu (veya ekrana tıklama)
- **Duraklat / Devam Et**: `P` tuşu
- **Ses Kontrolü**: Sağ üstteki ses butonu

## 🚀 Çalıştırma
Projeyi doğrudan açmak için `index.html` dosyasını herhangi bir web tarayıcısında açmanız yeterlidir.

Alternatif olarak yerel bir HTTP sunucusu ile çalıştırmak isterseniz:
```bash
python -m http.server 8085
```
Tarayıcınızdan `http://localhost:8085` adresine gidebilirsiniz.
