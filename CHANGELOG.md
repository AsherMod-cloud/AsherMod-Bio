# Changelog

## [Unreleased]

### Added

- Menambahkan CTA eksternal **AsherMod Bypass** menuju `https://ashermod-bypass.pages.dev` pada halaman utama.
- Menambahkan halaman `referral.html` dengan tiga referral shortlink: Safelinku, Adsafelink, dan Snacklink.
- Menambahkan fallback otomatis **Segera Hadir** ketika URL referral dikosongkan.
- Menambahkan theme toggle pada referral page yang mengikuti nilai `asher-theme` dari halaman utama.

### Changed

- Menambahkan visual accent khusus untuk CTA Bypass dan Referral Shortlink agar dapat dibedakan dari link komunitas biasa.
- Menambahkan link internal `/referral.html` pada daftar link utama.

### SEO

- Menambahkan meta description, robots directive, canonical URL, locale, Open Graph image metadata, Twitter Card image metadata, favicon JPEG, dan Apple touch icon pada halaman utama.
- Menambahkan meta description, robots directive, canonical URL, Open Graph/Twitter metadata, dan JSON-LD WebPage + ItemList pada `referral.html`.
- Menambahkan JSON-LD ProfilePage + Person dengan `sameAs` untuk channel resmi pada `index.html`.
- Menambahkan `sitemap.xml` untuk halaman publik utama dan referral.
- Menambahkan `robots.txt` dengan referensi sitemap serta pengecualian untuk halaman AsherGo dan file dokumentasi.
- Menetapkan `AsherGo.html` sebagai `noindex, nofollow` karena merupakan secret mini game, bukan landing page SEO.

- Menambahkan meta tag `google-site-verification` untuk property URL Prefix `https://asher-mod-bio.pages.dev/`.
- Memperbarui `SEO-GUIDE.md` dengan alur verifikasi URL Prefix dan troubleshooting error pengambilan sitemap pada Search Console.
