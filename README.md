# Zero Notification 🔔

<p align="center">
  <img src="screenshots/ic_launcher_round.png" width="140" alt="Zero Notification Logo"/>
</p>

<p align="center">
  <b>Pembaca notifikasi otomatis dengan Text-to-Speech</b><br/>
  Rasakan pengalaman seperti katalog Google Play langsung dari GitHub sebelum rilis resmi.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Android-35-green?style=flat-square&logo=android"/>
  <img src="https://img.shields.io/badge/Kotlin-1.9.24-blue?style=flat-square&logo=kotlin"/>
  <img src="https://img.shields.io/badge/Min%20SDK-24-orange?style=flat-square"/>
</p>

---

## 💡 Kenapa berguna

- Memastikan notifikasi penting tetap terdengar saat berkendara, berolahraga, atau layar terkunci.
- Mode headset/speaker terpisah supaya suara tidak bocor ke publik.
- Filter kata dan ban words menjaga privasi pesan yang tidak ingin dibacakan.
- Riwayat notifikasi membantu meninjau pesan yang pernah masuk.

## ✨ Fitur Utama

- Text-to-Speech untuk semua aplikasi yang Anda pilih.
- Mode Headset dan Mode Speaker dengan kontrol cepat via Quick Settings Tile.
- Filter Words dan Ban Words untuk sensor otomatis.
- Batas kata dan deteksi duplikasi agar TTS tetap ringkas.
- Riwayat notifikasi (Room DB) yang bisa dilihat ulang.
- Multi bahasa TTS, dukungan silent mode, opsi layar menyala, dan hentikan bacaan dengan goyang ponsel.

## 🖼️ Tampilan (Screenshots)

| Beranda | Pengaturan | Widget |
| --- | --- | --- |
| <img src="screenshots/main.png" alt="Tampilan utama Zero Notification" width="260"/> | <img src="screenshots/setting.png" alt="Pengaturan Zero Notification" width="260"/> | <img src="screenshots/widget.png" alt="Widget Zero Notification" width="260"/> |

## 🧭 Cara Pakai Singkat

1. Install APK dari GitHub Releases (atau build sendiri).
2. Buka Zero Notification dan ikuti intro untuk memberi izin Akses Notifikasi serta pengecualian baterai jika diperlukan.
3. Pilih aplikasi yang ingin dibacakan notifikasinya dan atur mode output (headset atau speaker).
4. Tambahkan filter/ban words jika ada kata yang tidak ingin dibacakan.
5. Uji dengan mengirim notifikasi dari aplikasi pilihan; TTS akan membacakan sesuai aturan yang diaktifkan.

## 🔔 Alur Notifikasi Singkat

1. NotificationListenerService menangkap notifikasi masuk.
2. Pengecekan kondisi: aplikasi terdaftar, mode senyap/layar, koneksi headset, duplikasi, serta ban words.
3. Jika lolos, pesan diproses (judul, isi, batas kata) lalu dikirim ke layanan TTS.
4. Suara diputar melalui speaker/headset dan disimpan ke riwayat.

## ⚙️ Izin & Kebutuhan

- Android 7.0 (API 24)+
- Akses Notifikasi (wajib)
- Text-to-Speech Engine (disarankan Google TTS)
- Pengecualian optimasi baterai (opsional, untuk memastikan layanan tetap aktif)

## ℹ️ Info Singkat

- App ini masih tahap pra-rilis. Jika menemukan bug atau punya masukan, buka tab Issues di GitHub.
- Semua data notifikasi hanya diproses di perangkat dan bisa disaring dengan filter/ban words untuk privasi.

<p align="center">
  Made with ❤️ oleh Zero Dev
</p>
