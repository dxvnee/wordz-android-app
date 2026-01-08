# 📘 Wordz - Aplikasi Pembelajaran Kosakata Bahasa Inggris

<div align="center">

![Wordz App](app/src/main/res/drawable/wordzwhite.png)

[![Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://www.android.com/)
[![Kotlin](https://img.shields.io/badge/Language-Kotlin-blue.svg)](https://kotlinlang.org/)
[![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-brightgreen.svg)](https://developer.android.com/jetpack/compose)
[![Room Database](https://img.shields.io/badge/Database-Room-orange.svg)](https://developer.android.com/training/data-storage/room)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

**Aplikasi pembelajaran kosakata yang membantu Anda menyimpan, mengelola, dan menghafal kosakata bahasa Inggris melalui fitur CRUD dan kuis interaktif**

[Fitur](#-fitur-utama) • [Teknologi](#-teknologi-yang-digunakan) • [Instalasi](#-instalasi) • [Penggunaan](#-cara-menggunakan) • [Kontribusi](#-kontribusi)

</div>

---

## 📋 Deskripsi

**Wordz** adalah aplikasi Android native yang dirancang untuk membantu pengguna mempelajari dan menghafal kosakata bahasa Inggris dengan cara yang personal dan efektif. Berbeda dengan aplikasi kosakata pada umumnya yang menggunakan daftar kata standar, Wordz memungkinkan pengguna untuk menambahkan kata-kata yang **benar-benar mereka temui** dalam kehidupan sehari-hari seperti dari buku, film, lagu, dokumentasi pemrograman, dan sumber lainnya.

### 🎯 Tujuan Aplikasi

- ✅ Menyimpan kosakata bahasa Inggris yang baru dipelajari secara personal
- ✅ Mendorong pembelajaran konsisten dan memori jangka panjang
- ✅ Mengubah pembelajaran kosakata menjadi pengalaman yang **aktif dan menyenangkan** melalui kuis
- ✅ Membantu pengguna **benar-benar mengingat** kosakata, bukan hanya menyimpannya

### 💡 Filosofi

> *"Kosakata tidak dimaksudkan untuk disimpan — tetapi untuk diingat."*

Wordz bertujuan menjadi **teman belajar kosakata yang sederhana, personal, dan efektif**.

---

## ✨ Fitur Utama

### 1️⃣ Manajemen Kosakata (CRUD)

Kelola koleksi kosakata Anda dengan mudah:

- **➕ Tambah Kata Baru**: Simpan kata bahasa Inggris beserta terjemahan dan catatan tambahan
- **👀 Lihat Daftar Kosakata**: Tampilkan semua kata yang telah disimpan dalam tampilan list atau grid
- **✏️ Edit Kosakata**: Ubah kata, terjemahan, atau catatan kapan saja
- **🗑️ Hapus Kosakata**: Hapus kata yang tidak lagi relevan
- **📅 Tanggal Penyimpanan**: Opsi untuk menyimpan tanggal penambahan kata

Semua kosakata bersifat **kustom dan personal**, berdasarkan kata-kata yang benar-benar ingin Anda pelajari.

### 2️⃣ Kuis Interaktif

Fitur kuis yang dihasilkan **sepenuhnya dari daftar kosakata Anda sendiri**:

- 🎮 Pilih terjemahan yang benar untuk sebuah kata
- 🎯 Tebak kata yang tepat berdasarkan terjemahannya
- 📊 Pelacakan skor (benar dan salah)
- 🎉 Layar hasil akhir dengan opsi berbagi skor
- 📱 Minimal 5 kata diperlukan untuk memulai kuis

**Tujuan Kuis:**
- Menguji retensi memori
- Memperkuat ingatan jangka panjang
- Membuat pembelajaran kosakata terasa seperti permainan, bukan hafalan paksa

### 3️⃣ Antarmuka Modern

- 🎨 Desain UI/UX modern dengan Material Design 3
- 🌈 Tema custom dengan skema warna ungu yang menarik
- 📱 Responsive design yang optimal untuk berbagai ukuran layar
- 🔄 Smooth navigation dengan Jetpack Navigation Component
- 💫 Splash screen dengan branding aplikasi

---

## 🛠️ Teknologi yang Digunakan

### Platform & Bahasa
- **Platform**: Android (API Level 23+)
- **Bahasa Pemrograman**: Kotlin
- **Min SDK**: 23 (Android 6.0 Marshmallow)
- **Target SDK**: 34 (Android 14)

### Android Jetpack Components
- **Jetpack Compose**: Modern UI toolkit untuk membangun native UI
- **Room Database**: Abstraksi database SQLite untuk penyimpanan lokal
- **ViewModel**: Mengelola data terkait UI dengan lifecycle-aware
- **Navigation Component**: Navigasi antar screen
- **DataStore**: Penyimpanan preferensi aplikasi
- **Lifecycle**: Komponen lifecycle-aware
- **Core-KTX**: Ekstensi Kotlin untuk Android framework

### Libraries & Dependencies
```gradle
- Jetpack Compose BOM 2023.08.00
- Material Design 3
- Room Database 2.6.1
- Navigation Compose 2.7.7
- DataStore Preferences 1.0.0
- Core Splashscreen 1.0.1
- Kotlin Coroutines
- KSP (Kotlin Symbol Processing)
```

### Arsitektur
- **Pattern**: MVVM (Model-View-ViewModel)
- **Database**: Room (SQLite)
- **Reactive Programming**: Kotlin Flow & StateFlow
- **Dependency Injection**: ViewModelFactory pattern

---

## 📦 Instalasi

### Prasyarat
Sebelum memulai, pastikan Anda telah menginstal:
- [Android Studio](https://developer.android.com/studio) (versi terbaru direkomendasikan)
- JDK 8 atau lebih tinggi
- Android SDK dengan API Level 23 atau lebih tinggi
- Gradle 8.2.2 atau kompatibel

### Langkah-langkah Instalasi

1. **Clone Repository**
   ```bash
   git clone https://github.com/dxvnee/wordz-android-app.git
   cd wordz-android-app
   ```

2. **Buka Proyek di Android Studio**
   - Buka Android Studio
   - Pilih `File` > `Open`
   - Navigasikan ke folder proyek yang telah di-clone
   - Klik `OK`

3. **Sync Gradle**
   - Android Studio akan otomatis melakukan Gradle sync
   - Jika tidak, klik `File` > `Sync Project with Gradle Files`
   - Tunggu hingga proses selesai

4. **Build Project**
   ```bash
   ./gradlew build
   ```

5. **Run Aplikasi**
   - Hubungkan device Android atau jalankan emulator
   - Klik tombol `Run` (ikon play hijau) di Android Studio
   - Atau gunakan command line:
   ```bash
   ./gradlew installDebug
   ```

### Build APK

Untuk membuat APK yang dapat diinstal:

**Debug APK:**
```bash
./gradlew assembleDebug
```
APK akan tersimpan di: `app/build/outputs/apk/debug/`

**Release APK:**
```bash
./gradlew assembleRelease
```
APK akan tersimpan di: `app/build/outputs/apk/release/`

---

## 📱 Cara Menggunakan

### 1. Menambah Kosakata Baru

1. Di halaman utama, ketuk tombol **floating action button** (ikon +) di pojok kanan bawah
2. Isi formulir:
   - **Words**: Masukkan kata dalam bahasa Inggris (contoh: "Table")
   - **Translate**: Masukkan terjemahan (contoh: "Meja")
   - **Notes**: Tambahkan catatan opsional (contoh: "Is a flat horizontal surface")
   - **Save Input Date**: Centang jika ingin menyimpan tanggal penambahan
3. Ketuk tombol **Add Words** untuk menyimpan

### 2. Melihat Daftar Kosakata

- Semua kosakata yang telah ditambahkan akan ditampilkan di halaman utama
- Ketuk ikon **list** atau **grid** di top bar untuk mengubah tampilan
- Setiap kartu kosakata menampilkan:
  - Kata dalam bahasa Inggris
  - Terjemahan
  - Catatan (jika ada)
  - Tanggal penambahan (jika disimpan)

### 3. Mengedit Kosakata

1. Ketuk kartu kosakata yang ingin diedit
2. Ubah informasi yang diperlukan
3. Ketuk tombol **Save** untuk menyimpan perubahan

### 4. Menghapus Kosakata

1. Ketuk kartu kosakata yang ingin dihapus
2. Ketuk ikon **menu** (titik tiga) di pojok kanan atas
3. Pilih **Delete Word**
4. Konfirmasi penghapusan

### 5. Memulai Kuis

1. Di halaman utama, pastikan Anda memiliki **minimal 5 kata** dalam daftar kosakata
2. Ketuk tombol **Quiz** dengan ikon panah
3. Jawab pertanyaan dengan memilih jawaban yang benar
4. Lihat skor Anda di akhir kuis
5. Bagikan hasil kuis Anda dengan tombol **Share**

---

## 📂 Struktur Proyek

```
wordz-android-app/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/org/d3if3121/wordz3/
│   │   │   │   ├── database/          # Room Database
│   │   │   │   │   ├── WordsDao.kt
│   │   │   │   │   └── WordsDb.kt
│   │   │   │   ├── model/             # Data Models
│   │   │   │   │   └── Words.kt
│   │   │   │   ├── navigation/        # Navigation
│   │   │   │   │   ├── NavGraph.kt
│   │   │   │   │   └── Screen.kt
│   │   │   │   ├── ui/
│   │   │   │   │   ├── screen/        # UI Screens
│   │   │   │   │   │   ├── MainScreen.kt
│   │   │   │   │   │   ├── DetailScreen.kt
│   │   │   │   │   │   ├── QuizScreen2.kt
│   │   │   │   │   │   ├── MainViewModel.kt
│   │   │   │   │   │   ├── DetailViewModel.kt
│   │   │   │   │   │   └── DisplayAlertDialog.kt
│   │   │   │   │   └── theme/         # UI Theme
│   │   │   │   │       ├── Color.kt
│   │   │   │   │       ├── Theme.kt
│   │   │   │   │       └── Type.kt
│   │   │   │   ├── util/              # Utilities
│   │   │   │   │   ├── SettingsDataStore.kt
│   │   │   │   │   └── ViewModelFactory.kt
│   │   │   │   └── MainActivity.kt
│   │   │   ├── res/                   # Resources
│   │   │   │   ├── drawable/
│   │   │   │   ├── mipmap/
│   │   │   │   ├── values/
│   │   │   │   └── xml/
│   │   │   └── AndroidManifest.xml
│   │   ├── androidTest/               # Android Tests
│   │   └── test/                      # Unit Tests
│   ├── build.gradle.kts
│   └── proguard-rules.pro
├── gradle/
├── build.gradle.kts
├── settings.gradle.kts
├── gradle.properties
├── gradlew
├── gradlew.bat
├── .gitignore
└── README.md
```

---

## 🗄️ Struktur Database

### Tabel: words

| Kolom | Tipe | Deskripsi |
|-------|------|-----------|
| id | Long (Primary Key) | ID unik untuk setiap kosakata (auto-increment) |
| word | String | Kata dalam bahasa Inggris |
| meaning | String | Terjemahan atau arti kata |
| note | String | Catatan tambahan (opsional) |
| dateAdded | String | Tanggal penambahan kata |

---

## 🎨 Screenshots

> **Catatan**: Tambahkan screenshot aplikasi Anda di sini untuk memberikan preview visual kepada pengguna

```
[Screenshot 1: Halaman Utama]
[Screenshot 2: Tambah Kata Baru]
[Screenshot 3: Kuis]
[Screenshot 4: Hasil Kuis]
```

---

## 🚀 Pengembangan Selanjutnya

Beberapa fitur yang direncanakan untuk versi mendatang:

- [ ] 📊 Statistik progress pembelajaran
- [ ] 🔔 Reminder kuis harian
- [ ] 🎚️ Level kesulitan kuis
- [ ] ☁️ Sinkronisasi cloud
- [ ] 🔊 Dukungan audio pronunciation
- [ ] 🌐 API untuk mendapatkan definisi kata otomatis
- [ ] 📈 Grafik perkembangan pembelajaran
- [ ] 🏆 Sistem achievement dan badges
- [ ] 🌙 Dark mode
- [ ] 🔍 Fitur pencarian kata
- [ ] 📤 Export/Import data kosakata
- [ ] 🎯 Kategori kata (noun, verb, adjective, dll.)

---

## 🎯 Target Pengguna

Aplikasi ini cocok untuk:

- 📚 **Pelajar dan Mahasiswa**: Yang ingin memperkaya kosakata bahasa Inggris
- 💻 **Developer**: Yang sering menemui istilah baru dalam dokumentasi pemrograman
- 📖 **Pembaca**: Yang ingin menyimpan kata-kata baru dari buku atau artikel
- 🎬 **Penggemar Film/Series**: Yang ingin belajar dari subtitle atau dialog
- 🎵 **Pecinta Musik**: Yang ingin memahami lirik lagu berbahasa Inggris
- 👥 **Siapa Saja**: Yang ingin membangun kosakata secara konsisten dan menyenangkan

---

## 🤝 Kontribusi

Kontribusi selalu diterima dengan tangan terbuka! Jika Anda ingin berkontribusi:

1. **Fork** repository ini
2. **Create** branch baru (`git checkout -b feature/AmazingFeature`)
3. **Commit** perubahan Anda (`git commit -m 'Add some AmazingFeature'`)
4. **Push** ke branch (`git push origin feature/AmazingFeature`)
5. **Open** Pull Request

### Cara Berkontribusi

- 🐛 **Report Bugs**: Buat issue baru dengan label `bug`
- 💡 **Request Features**: Buat issue baru dengan label `enhancement`
- 📝 **Improve Documentation**: Perbaiki atau tambahkan dokumentasi
- 🔧 **Fix Issues**: Pilih issue yang ada dan kerjakan
- ✨ **Add Features**: Implementasikan fitur baru

### Code Style

- Ikuti [Kotlin Coding Conventions](https://kotlinlang.org/docs/coding-conventions.html)
- Gunakan meaningful variable dan function names
- Tambahkan komentar untuk logika yang kompleks
- Pastikan kode Anda ter-format dengan baik

---

## 📄 Lisensi

Project ini dilisensikan di bawah [MIT License](LICENSE). Anda bebas untuk:

- ✅ Menggunakan secara komersial
- ✅ Memodifikasi
- ✅ Mendistribusikan
- ✅ Menggunakan secara pribadi

Dengan syarat:
- Sertakan lisensi dan copyright notice dalam salinan software

---

## 👨‍💻 Author

Dikembangkan oleh **dxvnee** sebagai proyek pembelajaran dan eksplorasi dalam software engineering.

### Connect

- 🔗 GitHub: [@dxvnee](https://github.com/dxvnee)

---

## 🙏 Acknowledgments

- **Android Team**: Untuk platform dan tools yang luar biasa
- **JetBrains**: Untuk bahasa Kotlin yang powerful
- **Material Design**: Untuk design system yang indah
- **Open Source Community**: Untuk semua library dan resource yang digunakan

---

## 📞 Support

Jika Anda mengalami masalah atau memiliki pertanyaan:

1. Cek [Issues](https://github.com/dxvnee/wordz-android-app/issues) yang sudah ada
2. Buat [New Issue](https://github.com/dxvnee/wordz-android-app/issues/new) jika belum ada
3. Berikan detail sebanyak mungkin tentang masalah Anda

---

## ⭐ Star History

Jika proyek ini membantu Anda, jangan lupa untuk memberikan ⭐ pada repository ini!

---

<div align="center">

**Made with ❤️ and ☕ by dxvnee**

**Happy Learning! 📚✨**

</div>
