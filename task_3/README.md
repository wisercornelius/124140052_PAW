# Tugas Individu 3 — Pemrograman Web

Halaman web sederhana dengan dua halaman: **pendaftaran** dan **detail pendaftar**.

## Struktur File

| File          | Keterangan                                              |
| ------------- | ------------------------------------------------------- |
| `index.html`  | Halaman pendaftaran (form dengan `method="GET"`)        |
| `detail.html` | Halaman detail informasi pendaftar (data dummy)         |
| `style.css`   | Stylesheet layout, box, tabel, dan form untuk 2 halaman |

## Cara Menjalankan

Buka `index.html` di browser, isi formulir, lalu klik **Lihat Detail**. Browser akan
membuka `detail.html` dengan query string berisi data yang diisi.

> Sesuai instruksi tugas, halaman detail **tidak menangkap/memproses** query string.
> Data yang ditampilkan adalah data dummy.

## Rancangan Query String

Form menggunakan `method="GET"` dengan `action="detail.html"`, sehingga data dikirim
sebagai pasangan `name=value` yang dipisahkan `&`:

```text
detail.html?nama=Cornelius+Adhi+Prasetya&nim=124140052&kelas=RA&prodi=Teknik+Informatika&email=cornelius.prasetya%40student.ac.id&telepon=081234567890&jenis_kelamin=Laki-laki&tanggal_lahir=2005-08-12&alamat=Jl.+Soekarno-Hatta+No.+12%2C+Bandar+Lampung
```

| Parameter       | Field Form      | Contoh Nilai            |
| --------------- | --------------- | ----------------------- |
| `nama`          | Nama Lengkap    | `Cornelius Adhi Prasetya` |
| `nim`           | NIM             | `124140052`             |
| `kelas`         | Kelas           | `RA`                    |
| `prodi`         | Program Studi   | `Teknik Informatika`    |
| `email`         | Email           | `cornelius.prasetya@student.ac.id` |
| `telepon`       | No. HP          | `081234567890`          |
| `jenis_kelamin` | Jenis Kelamin   | `Laki-laki`             |
| `tanggal_lahir` | Tanggal Lahir   | `2005-08-12`            |
| `alamat`        | Alamat          | `Jl. Soekarno-Hatta No. 12, Bandar Lampung` |

## Selector CSS yang Digunakan

1. **Element** — `body`, `table`, `th`, `td`, `input`, `textarea`, `select`
2. **Class** — `.page`, `.card`, `.card-head`, `.field`, `.btn`, `.btn-primary`, `.badge`
3. **ID** — `#form-pendaftaran`
4. **Descendant / child** — `.field > label`, `.table-wrap table`, `tbody tr:hover td`
5. **Pseudo-class** — `:focus`, `:hover`, `:active`, `:nth-child(even)`, `:last-child`
6. **Attribute** — `input[type="email"]`, `input[type="radio"]`

## Pengumpulan

- Simpan seluruh file di folder **`task_3`** pada repository GitHub masing-masing.
- Ekspor dokumentasi/screenshot tugas menjadi PDF dengan format nama:
  `kelas-Nama-Nim-Tugas3-Pemweb.pdf`
  Contoh: `RA-Cornelius Adhi Prasetya-124140052-Tugas3-Pemweb.pdf`
