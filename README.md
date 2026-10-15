# 2k48

Mobil uyumlu 2048 oyunu. Tasarım: Hakan Korkmaz.

Statik site: derleme adımı yok.

## Vercel'e yükleme
1. Bu klasörü GitHub'a gönder, Vercel'de **Add New → Project** ile içe aktar.
   Framework Preset: **Other**. Build Command ve Output Directory boş kalsın.
2. Ya da terminalde: `npx vercel --prod` (klasörün içinde).

## Dosyalar
- `index.html`: oyunun tamamı (HTML, CSS, JS)
- `favicon.svg`, `favicon-32.png`: tarayıcı sekmesi ikonu
- `apple-touch-icon.png`: iPhone ana ekran ikonu
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `manifest.webmanifest`: Android ana ekran / uygulama olarak yükleme
- `icon.svg`: logonun vektör hali
- `vercel.json`: güvenlik başlıkları ve temiz URL ayarı

Skorlar (en fazla 50) ve ses tercihi ziyaretçinin tarayıcısında (localStorage) tutulur. Sesler WebAudio ile üretilir, ses dosyası yoktur.
