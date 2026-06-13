# 📝 SimpleNote-UnitTest

Proyek sederhana berisi UI testing menggunakan **Espresso** untuk aplikasi catatan (Notes) di Android. Pengujian mencakup penambahan catatan baru dan validasi input pada form.

## 🧪 Test Cases

### 1. `testAddNote`
Menguji penambahan catatan baru:
- Mengisi field judul dan konten
- Klik tombol tambah
- Memastikan catatan tampil di RecyclerView (judul & isi sesuai input)
- Memastikan tampilan "Tidak ada catatan" tersembunyi

### 2. `testInputValidation`
Menguji validasi input saat menambah catatan:
- Klik tombol tambah tanpa input apapun → RecyclerView tetap kosong
- Isi judul saja tanpa konten → RecyclerView tetap kosong
- Isi konten saja tanpa judul → RecyclerView tetap kosong

## 🛠️ Komponen Tambahan

- **`RecyclerViewItemCountAssertion`** — custom assertion untuk memverifikasi jumlah item di RecyclerView
- **`ToastMatcher`** — custom matcher untuk memverifikasi tampilan Toast message

## ⚙️ Teknologi

- Java
- Espresso (`androidx.test.espresso`)
- AndroidJUnit4

## ▶️ Cara Menjalankan

1. Buka project di Android Studio
2. Pastikan emulator/device aktif
3. Klik kanan pada file test → **Run 'MainActivityTest'**
