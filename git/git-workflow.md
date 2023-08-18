# Seputar Git
![Git workflow](images/git-workflow.png 'Git workflow')

Dari gambar di atas, di Git terdapat dua sumber repositori, yaitu repositori lokal dan repositori remot. Kedua sumber harus sinkron.
- Repositori lokal, adalah repositori yang berada di komputer kita.
- Repositori remot, adalah repositori di luar komputer kita (server).

## Tentang Repositori Lokal
Repositori di sisi komputer kita (lokal), dibagi menjadi tiga tempat atau area.

1. Working directory ⇒ tempat di mana berkas-berkas proyek kita berada
2. Staging area ⇒ tempat di mana berkas-berkas proyek yang siap disimpan ke repositori lokal sebagai **snapshot**
   Mulai sekarang dan seterusnya, **snapshot** kita sebut sebagai **commit**
3. Local repository ⇒ repositori yang ada di komputer kita, di mana berisi kumpulan **commit** yang telah kita buat

## Alur Kerja
### Sinkronisasi antara Repositori Lokal dan Remot
Semua perintah yang akan dibahas harus di awali dengan `git`, misalnya `git add .`
- `push` ⇒ mengunggah **commit** yang berada di repo lokal menuju repo remot
- `pull` ⇒ mengunduh **commit** dari repo remot menuju repo lokal, lalu langsung digabungkan ke **staging area**
- `fetch` ⇒ mengunduh **commit** dari repo remot menuju repo lokal saja. Tidak menyentuh **staging area** kecuali dilakukan secara manual dengan perintah `merge`
