# Changelog

> **Catatan:** Changelog ini mulai aktif dipelihara sejak **14 Agustus 2026**. Perubahan sebelum tanggal tersebut tidak tercatat secara rinci.

## [1.0.0] - 11 September 2026

Rilis stabil pertama project bio link AsherMod setelah penambahan fitur referral, CTA AsherMod Bypass, dan optimasi SEO.

### Added 

- Menambahkan CTA eksternal **AsherMod Bypass** menuju `https://ashermod-bypass.pages.dev` pada halaman utama.
- Menambahkan halaman `referral.html` dengan tiga referral shortlink: Safelinku, Adsafelink, dan Snacklink.
- Menambahkan fallback otomatis **Segera Hadir** ketika URL referral dikosongkan.
- Menambahkan theme toggle pada referral page yang mengikuti nilai `asher-theme` dari halaman utama.
- Menambahkan halaman **`404.html`** dengan tema visual yang konsisten dengan halaman utama (Space Grotesk + Inter, gradient background, noise overlay, animated glow).
- Menambahkan theme toggle pada halaman 404 yang sinkron dengan `asher-theme` di `localStorage`.
- Menambahkan dua tombol navigasi pada halaman 404: **Kembali ke Beranda** dan **Lihat Referral**.
- Menambahkan dukungan `lite-mode` pada halaman 404 untuk WebView/1DM/low-end device.
- Menambahkan dukungan `prefers-reduced-motion` pada halaman 404.
- Menambahkan script anti long-press (`contextmenu` blocker) pada avatar container di halaman utama.

### Changed

- Menambahkan visual accent khusus untuk CTA Bypass dan Referral Shortlink agar dapat dibedakan dari link komunitas biasa.
- Menambahkan link internal `/referral.html` pada daftar link utama.
- Mengubah halaman `referral.html` dari daftar shortlink sederhana menjadi halaman promosi platform penghasil uang yang direkomendasikan AsherMod.
- Menambahkan tagline, deskripsi, dan daftar benefit pada setiap platform referral agar manfaat masing-masing layanan lebih jelas sebelum pengguna membuka link.
- Mengubah CTA referral menjadi tombol khusus **Coba [Platform] →** agar lebih sesuai dengan fungsi halaman promosi.
- Menambahkan blok informasi di bagian bawah yang menjelaskan bahwa link pada halaman merupakan **Referral Link** dan penggunaannya membantu mendukung pengembangan project AsherMod.
- Menambahkan atribut `rel="sponsored noopener noreferrer"` pada link referral.
- Mengubah title halaman utama menjadi **AsherMod — Bio Link** agar identitas halaman lebih ringkas dan fokus.
- Mengganti favicon halaman utama menggunakan **profile image AsherMod**.
- Memperbarui Apple Touch Icon agar menggunakan profile image yang sama.
- Menggunakan `profile.jpg` sebagai profile image untuk favicon dan metadata Open Graph/Twitter pada halaman terkait.
- Menyempurnakan theme toggle pada `referral.html` agar identik dengan `index.html` (ikon SVG sun/moon, animasi rotasi, dan transisi bounce).
- Mengganti hero section `referral.html` menjadi **AsherMod Referral** dengan deskripsi promosi platform penghasilan tambahan.
- Menambahkan anti long-press (`-webkit-touch-callout`, `-webkit-user-drag`, `draggable="false"`, `oncontextmenu`) pada avatar dan gambar profil di halaman utama untuk mencegah munculnya menu "Simpan Gambar" saat ditekan lama.
- Menambahkan `user-select: none` secara global pada `index.html` dengan pengecualian untuk elemen yang perlu tetap bisa disalin (`.dana-number`, `.profile-bio`, `.footer-url`).
- Menonaktifkan tap highlight biru (`-webkit-tap-highlight-color: transparent`) pada seluruh elemen interaktif di `index.html` dan `referral.html`.

### SEO

- Menambahkan meta description, robots directive, canonical URL, locale, Open Graph image metadata, Twitter Card image metadata, favicon JPEG, dan Apple touch icon pada halaman utama.
- Menambahkan meta description, robots directive, canonical URL, Open Graph/Twitter metadata, dan JSON-LD WebPage + ItemList pada `referral.html`.
- Menambahkan JSON-LD ProfilePage + Person dengan `sameAs` untuk channel resmi pada `index.html`.
- Menambahkan `sitemap.xml` untuk halaman publik utama dan referral.
- Menambahkan `robots.txt` dengan referensi sitemap serta pengecualian untuk halaman AsherGo dan file dokumentasi.
- Menetapkan `AsherGo.html` sebagai `noindex, nofollow` karena merupakan secret mini game, bukan landing page SEO.
- Menetapkan `404.html` sebagai `noindex, follow` agar tidak terindeks namun tetap mengikuti link di dalamnya.
- Memperbarui meta title dan description pada `referral.html` menjadi **AsherMod Referral** dengan deskripsi yang berfokus pada penghasilan tambahan dari aktivitas online.
- Menambahkan meta tag `google-site-verification` untuk property URL Prefix `https://asher-mod-bio.pages.dev/`.
- Memperbarui `SEO-GUIDE.md` dengan alur verifikasi URL Prefix dan troubleshooting error pengambilan sitemap pada Search Console.