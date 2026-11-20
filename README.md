# Upgrade XP · Valencia düğün mekânları

Kapalı devre çalışma sayfası. Statik site, derleme adımı yok. İki yerde yayımlanır:

- GitHub Pages: https://gokhansunar.github.io/upgrade-xp-valencia/ (Türkiye'den bu adres kullanılır; vercel.app uzantısı Türkiye'deki bağlantılarda açılmıyor)
- Vercel: https://upgrade-xp-valencia.vercel.app/

- `index.html`: uygulama (mekânlar, catering, konaklama, transfer, Video Stüdyo)
- `img/`: mekân fotoğrafları (Wikimedia Commons ve Upgrade XP kataloğu)
- `vercel.json`: Vercel için arama motorlarına kapalı (noindex) başlıklar ve önbellek ayarı; sayfanın kendisinde de noindex etiketi var
- `.nojekyll`: GitHub Pages dosyaları olduğu gibi yayımlasın diye

Fotoğraf ve video yükleme, kayıt ve Claude kontrolleri Claude'daki sürümde yapılır. Bu web sürümünde yapılan değişiklikler yalnızca o tarayıcıda kalır.
