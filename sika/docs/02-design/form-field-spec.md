# Form Field Specification - form-mahasiswa.html

| Field (name) | Tujuan | Type HTML | Wajib | Batas | Klasifikasi data |
|--------------|--------|-----------|-------|-------|------------------|
| nim | Identitas unik mahasiswa | text | Ya | minlength 8, maxlength 15 | Internal |
| nama | Nama lengkap | text | Ya | minlength 3 | Pribadi |
| email | Kontak surel | email | Ya | format email | Pribadi |
| prodi | Program studi | select (TI, SI) | Ya | nilai dari daftar | Internal |
| angkatan | Tahun masuk | number | Ya | min 2020, max 2030 | Internal |
| status | Status akademik | radio (aktif, nonaktif) | Ya (default aktif) | 2 pilihan | Internal |

## Data minimization
Hanya enam field di atas yang dikumpulkan karena dibutuhkan use case FR-03. Tidak ada field alamat, tanggal lahir, NIK, atau password.

## Catatan keamanan
- Method `post` dan `action="#"` (persiapan Bab 6).
- Validasi HTML5 hanya lapisan usability; validasi ulang wajib di server (Bab 6).
- Tidak ada hidden input.
