# Rekod Kedatangan (app boleh dipasang di hp)

Folder ini ialah app lengkap. Tiada pelayan atau pemasangan diperlukan. Anda hanya perlu letakkan semua fail di tapak web yang menyokong HTTPS, kemudian pasang di hp.

## Fail

- `index.html` : app itu sendiri
- `manifest.webmanifest` : nama, warna dan ikon app
- `sw.js` : membolehkan app dibuka tanpa internet selepas dibuka sekali
- `icon-192.png`, `icon-512.png`, `icon-maskable-512.png`, `apple-touch-icon.png` : ikon

Letakkan semua fail dalam satu folder yang sama. Jangan tukar nama fail.

## Langkah 1: letak di tapak web (pilih satu)

**Netlify (paling mudah)**
1. Buka Netlify Drop (app.netlify.com/drop) dan log masuk atau daftar percuma.
2. Seret folder `kedatangan-pwa` (bukan fail zip) ke halaman itu.
3. Anda akan dapat alamat `https://...netlify.app`. Itulah alamat app anda.

**GitHub Pages**
1. Buat repositori awam baharu di GitHub dan muat naik semua fail ke bahagian paling atas repositori.
2. Pergi ke Settings, Pages, pilih cabang `main` dan folder `/ (root)`, kemudian Save.
3. Selepas beberapa minit, alamat `https://nama-anda.github.io/nama-repo/` akan aktif.

## Langkah 2: pasang di hp

**Android (Chrome)**
1. Buka alamat app di Chrome.
2. Tekan menu tiga titik, kemudian "Install app" atau "Add to Home screen".

**iPhone (Safari)**
1. Buka alamat app di Safari.
2. Tekan butang Kongsi, kemudian "Add to Home Screen".

Selepas itu, ikon "Kedatangan" muncul di skrin utama dan app terbuka tanpa bar pelayar.

## Perkara penting tentang data

- Data disimpan dalam hp anda sahaja, bukan di tapak web. Tapak web hanya menyimpan fail app.
- Rekod tidak dikongsi antara peranti. Kalau anda pasang di dua hp, setiap satu ada rekodnya sendiri.
- Di iPhone, app yang dipasang di skrin utama mempunyai simpanan berasingan daripada Safari. Masukkan nama dan rekod selepas anda pasang app, bukan sebelum itu.
- Kalau anda kosongkan data tapak atau buang app, rekod hilang. Gunakan butang "Data CSV" untuk salin sandaran ke Notes atau e-mel dari semasa ke semasa.

## Kemas kini app

Ganti fail di tapak web dengan versi baharu. Kalau perubahan tidak muncul, tukar `kedatangan-v1` kepada `kedatangan-v2` dalam `sw.js` sebelum muat naik.
