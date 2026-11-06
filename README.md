# 🎮 Zıplama Macerası (Jump Runner)

HTML5 Canvas ve saf JavaScript ile geliştirilmiş, harici kütüphane gerektirmeyen klasik sonsuz koşu & zıplama oyunu.

## ✨ Özellikler
- **Saf Web Teknolojisi**: Harici hiçbir kütüphane/paket gerekmez (`HTML5 Canvas`, `Vanilla JS`, `CSS3`).
- **🦘 Çift Zıplama (Double Jump)**: Karakter havadayken ekstra bir kez daha zıplayabilir; özel enerji halkası efekti ve sesi eşlik eder.
- **🛹 Eğilme & Kayma Mekaniği (Duck & Slide)**: Karakter eğilerek aerodinamik kayma pozisyonu alır, toz bulutları çıkarır ve havadaki engellerin altından güvenle geçer.
- **🦅 Uçan Havada Asılı Engeller (Siber Drone)**: Zıplayarak aşılamayan, altındaki güvenli koridordan yalnızca eğilerek geçilebilen uçan engeller.
- **🪙 Altın Toplama & Ödül Sistemi**: Zemin üstünde, havada ve uçan engellerin altında toplanabilen altınlar (`+25 Skor`, `🪙 Altın Sayacı` ve özel çınlama sesi).
- **🌅 Gece - Gündüz Döngüsü**: Dinamik ve yaşayan atmosfer (Gündüz ☀️ -> Gün Batımı 🌇 -> Yıldızlı Gece ve Ay 🌙 -> Şafak 🌄).
- **🎵 Zengin Web Audio API Sesleri**: Zıplama, çift zıplama, kayma, altın toplama, skor ve çarpışma sesleri (harici ses dosyası indirilmesi gerekmez).
- **Akıcı Parçacık Animasyonları**: Zıplama/iniş tozları, çift zıplama halkası, altın ışıltıları, kayma izleri ve çarpışma patlaması.
- **Kademeli Zorluk**: Skor yükseldikçe oyun hızı dengeli bir tempoda artar.
- **Yüksek Skor Kaydı**: En yüksek skor tarayıcı hafızasında (`localStorage`) saklanır.
- **Mobil & Dokunmatik Uyumlu**: Hem klavye hem mobil dokunmatik butonları (Zıpla & Eğil) destekler.

## 🕹️ Kontroller
- **Zıplama / Çift Zıplama**: `Space`, `W` veya `Yukarı Ok (↑)` tuşu (veya ekrandaki Zıpla butonu / tık)
- **Eğilme / Kayma**: `S` veya `Aşağı Ok (↓)` tuşu (basılı tutun) (veya ekrandaki Eğil butonu)
- **Hızlı İniş (Fast-fall)**: Havada iken `S` veya `Aşağı Ok (↓)` basıldığında yere hızlı iniş yapar.
- **Duraklat / Devam Et**: `P` tuşu
- **Ses Kontrolü**: Sağ üstteki ses butonu

## 🚀 Çalıştırma
Projeyi doğrudan açmak için `index.html` dosyasını herhangi bir web tarayıcısında açmanız yeterlidir.

Alternatif olarak yerel bir HTTP sunucusu ile çalıştırmak isterseniz:
```bash
python -m http.server 8085
```
Tarayıcınızdan `http://localhost:8085` adresine gidebilirsiniz.
