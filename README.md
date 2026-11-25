# Pengukur Rute Lari Wanusobo (Android)

Project Android Studio sederhana yang membungkus aplikasi HTML/JavaScript dalam Android WebView.

## Membuka dan mengedit kode
1. Ekstrak ZIP.
2. Buka folder `PengukurRuteWanusobo` melalui Android Studio.
3. Tunggu Gradle Sync selesai.
4. Untuk mengubah tampilan, peta, perhitungan jarak, atau fitur web, edit `app/src/main/assets/index.html`.
5. Untuk mengubah perilaku Android, edit `app/src/main/java/id/wanusobo/pengukurrute/MainActivity.kt`.
6. Build APK melalui **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

APK hasil build biasanya berada di `app/build/outputs/apk/debug/app-debug.apk`.

## Catatan fungsi
- Mode Bebas mengukur garis lurus antar titik yang dipilih.
- Mode Ikuti Jalan memakai layanan publik OSRM dengan profil `driving` karena server demo OSRM umumnya menyediakan profil kendaraan, bukan pejalan kaki. Hasilnya bukan rute lari/jalan kaki yang dijamin aman atau akurat untuk gang dan jalan setapak.
- Peta dan layanan rute membutuhkan internet.
- Jika OSRM gagal, aplikasi otomatis kembali ke garis lurus antar titik.
