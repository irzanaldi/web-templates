# Template

Koleksi template / starter web (UI kit dan admin dashboard) dari berbagai stack.

## Isi

| Folder | Stack | Keterangan |
|--------|-------|------------|
| `Source/` | Laravel + Vite/Tailwind | Admin dashboard "Midone/Rubick" versi Laravel |
| `midonelaravel-502/` | Laravel | Beberapa varian tema Midone (Enigma, Icewall, Tinker, Rubick) |
| `material-dashboard-react-main/` | React | Material Dashboard React |
| `argon-flutter-master/` | Flutter | Argon UI kit untuk Flutter |
| `template-rubick-midone-livewire/` | Laravel + Livewire | Repo Git terpisah milik sendiri — sengaja di-exclude dari pack ini |

## Cara Setup

Ini adalah kumpulan template UI/starter. Pilih satu template, lalu jalankan dari dalam folder-nya masing-masing sesuai stack.

### Template Laravel (`Source/`, atau salah satu di `midonelaravel-502/.../Source/`)

```bash
cd Source            # atau path template Laravel yang dipilih

composer install
npm install
cp .env.example .env   # mulai dari contoh, jangan pakai .env asli
php artisan key:generate
php artisan migrate    # opsional, set koneksi DB di .env dulu
npm run dev
php artisan serve
```

### Template React (`material-dashboard-react-main/`)

```bash
cd material-dashboard-react-main
npm install
npm start
```

### Template Flutter (`argon-flutter-master/`)

```bash
cd argon-flutter-master
flutter pub get
flutter run
```

> Catatan keamanan: Semua file `.env` asli TIDAK ikut di-commit karena berisi kredensial. Selalu mulai dari `.env.example`. Folder `template-rubick-midone-livewire/` adalah repository Git tersendiri (punya remote sendiri), sehingga sengaja di-exclude dari pack ini.
