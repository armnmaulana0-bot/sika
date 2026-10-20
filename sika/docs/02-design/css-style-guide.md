# CSS Style Guide (Bab 3)

## Design tokens
| Token | Nilai | Fungsi |
|-------|-------|--------|
| --primary | #1d4ed8 | Navigasi, tombol, judul header |
| --primary-dark | #1e40af | Hover/focus/aktif |
| --surface | #ffffff | Kartu, form, tabel |
| --background | #f3f4f6 | Latar halaman |
| --text | #1f2937 | Teks utama |
| --muted | #4b5563 | Teks sekunder (kontras cukup) |
| --border | #d1d5db | Garis |
| --focus | #f59e0b | Outline focus 3px |
| --error / --success | #b91c1c / #166534 | Status (selalu dengan border/teks) |
| --radius | .75rem | Sudut kartu |
| --space-1..4 | .5 / 1 / 1.5 / 2 rem | Spacing konsisten |

## Tipografi
Arial, Helvetica, sans-serif; body 1rem, line-height 1.6; h1 1.75rem, h2 1.4rem, h3 1.15rem.

## Layout
- `.container`: `width: min(100% - 2rem, 1100px)`, dipusatkan.
- Flexbox: navigasi (`nav ul`) dan `.actions` (satu dimensi).
- Grid: `.dashboard-grid`, `.profile`, `.form-row` (dua dimensi).

## Komponen dan penamaan class
`.container`, `.card`, `.dashboard-grid`, `.notice`, `.profile`, `.profile-info`, `.table-wrapper`, `.form-row`, `.form-group`, `.actions`, `.hint`, `.page-title`, `button.secondary`, `label.inline`.

## Breakpoint (dipilih berdasarkan perilaku layout)
| Min-width | Perubahan |
|-----------|-----------|
| base (mobile) | 1 kolom |
| 640px | dashboard 2 kolom |
| 700px | profil: foto + info berdampingan |
| 768px | form 2 kolom |
| 960px | dashboard 3 kolom |
| max 640px | menu navigasi menjadi vertikal |

## Urutan file CSS
Reset/Base, Variables, Typography, Layout, Components, Forms & Tables, Media Queries.
