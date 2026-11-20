# Upgrade XP · Valencia düğün mekânları

Kapalı devre çalışma sayfası. Statik site, derleme adımı yok. İki yerde yayımlanır:

- GitHub Pages: https://gokhansunar.github.io/upgrade-xp-valencia/ (Türkiye'den bu adres kullanılır; vercel.app uzantısı Türkiye'deki bağlantılarda açılmıyor)
- Vercel: https://upgrade-xp-valencia.vercel.app/

- `index.html`: giriş kodu ekranı; uygulama (mekânlar, catering, konaklama, transfer, Video Stüdyo) bu dosyanın içinde şifreli durur
- `img/`: mekân fotoğrafları, şifreli (`.bin`)
- `vercel.json`: Vercel için arama motorlarına kapalı (noindex) başlıklar ve önbellek ayarı; sayfanın kendisinde de noindex etiketi var
- `.nojekyll`: GitHub Pages dosyaları olduğu gibi yayımlasın diye

Fotoğraf ve video yükleme, kayıt ve Claude kontrolleri Claude'daki sürümde yapılır. Bu web sürümünde yapılan değişiklikler yalnızca o tarayıcıda kalır.

## Giriş kodu

Sitenin içeriği ve fotoğrafları giriş koduyla şifrelenmiştir (AES-GCM, anahtar PBKDF2-SHA256 ile koddan türetilir). Kod bu depoda yer almaz. Kod girilmeden sayfada ve depoda yalnızca şifreli veri bulunur. Kod her cihazda bir kez sorulur, sonra o tarayıcıda hatırlanır.
