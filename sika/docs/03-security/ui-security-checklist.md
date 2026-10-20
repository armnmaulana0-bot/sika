# UI Security Checklist (Bab 2 + pembaruan Bab 3)

| No | Pemeriksaan | Status | Catatan / bukti |
|----|-------------|--------|-----------------|
| 1 | Setiap data yang tampil/dikumpulkan dibutuhkan use case | [x] | Lihat ui-requirement-map.md |
| 2 | Hanya data dummy (Andi Saputra, andi@example.com) | [x] | Isi file HTML |
| 3 | Tidak ada credential/API key/token/password di HTML, CSS, komentar | [x] | Source review |
| 4 | Form memakai POST, tidak ada data sensitif di URL | [x] | method="post" |
| 5 | Tidak ada hidden input; dipahami tetap terlihat di DevTools | [x] | - |
| 6 | Validasi HTML5 dipahami hanya lapisan usability | [x] | Validasi server wajib di Bab 6 |
| 7 | Tidak ada elemen sensitif yang hanya disembunyikan dengan CSS | [x] | Tidak ada display:none untuk data |
| 8 | Stylesheet/pseudo-element tidak memuat rahasia | [x] | style.css hanya presentasi |
| 9 | Tombol/fitur administratif = keputusan UI, bukan authorization | [x] | Authorization server-side dibangun di bab berikutnya |
| 10 | Focus state terlihat; status tidak hanya warna | [x] | Outline 3px; border + teks hint; link aktif bergaris bawah |
| 11 | Responsif tidak menyembunyikan informasi penting | [x] | Tabel memakai scroll horizontal, bukan disembunyikan |

## Potensi paparan data client-side yang dicegah (min. 2)
1. Tidak menaruh data pribadi nyata pada HTML/screenshot (memakai data dummy).
2. Tidak menaruh token/credential pada komentar HTML atau hidden input.
3. Tidak menyembunyikan data dengan CSS sebagai pengganti kontrol akses.
